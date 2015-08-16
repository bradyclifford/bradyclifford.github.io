---
published: true
layout: post
title: "Using Components and Resolves in UI-Router States"
category: JavaScript
tags: AngularJs
---

Adding to the **Component Pattern** in relation to AngluarJs and taking excerpts from this article: [component-paradigm](https://medium.com/@tomastrajan/component-paradigm-cf32e94ba78b)
 
Quick review... The importance of **controllerAs** and **bindToController** property in your directive / component.
[bindToController](http://blog.thoughtram.io/angularjs/2015/01/02/exploring-angular-1.3-bindToController.html)
 
In summary, the **bindToController** property helps in situations where we want to pass something to the directive’s isolated scope from parent component. When used, properties from isolated scope will be automatically bound to controller’s this.
 
The example below is referencing an inline template instead of a templateUrl in the ui-router state configuration.

```
$stateProvider
  .state('patients.patient.state', {
    url: /patient/:patientId',
    template: '<div state-patient></div>',
    resolve: {
      // ...
    },
  });
```
 
The problem with this is how do we inject our resolve data into the controller which is now not there?
 
Instead of injecting the resolved dependency data into the directive's controller, load it into a service.  Unfortunately I am not a fan of this approach.  It feels too much like scope inheritance...
 
```
.state(''patients.patient.state', {
    url: /patient/:patientId',
    template: '<div state-patient></div>',
    resolve: {
        init: function($stateParams, patientResource) {
            return patientResource.init($stateParams.itemId);
        }
    }
});
```

For details on this pattern, see the article below.
The examples are written in ES6, but the concept can be still be applied to our ES5 code base. [model-pattern-for-angular-js](https://medium.com/@tomastrajan/model-pattern-for-angular-js-67494389d6f)
 
Note that this is one way of tackling this problem.  I do not agree 100% with this approach but it does lay down the concept and possible alternatives.
