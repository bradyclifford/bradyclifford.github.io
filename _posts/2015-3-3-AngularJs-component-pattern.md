---
layout: post
title: AngularJs and the Component Pattern
category: JavaScript
tags: AngularJs
---
A few tips and a few standards related to using the component pattern with AngularJs.

Use one-way binding where possible.
Don’t use ng-controllers; instead modularize your code into directives; see attached document and link.  Also see example below.
•        Reduce your reference to $scope.  Instead use ControllerAs with vm.
•        Utilize the PubSub pattern; communicate between directives (components) with loosely coupled events.
•        Reference the John Papa AngularJS Style Guide until a AMDS AngularJS Style Guide can be constructed.
•        Keep AngularJs 2.0 in the back of your mind while writing your AngularJs apps. http://youtu.be/uD6Okha_Yj0 
•        For further Reference concerning these patterns, see the following post.

