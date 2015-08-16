---
layout: post
title: AngularJs and the Component Pattern
category: JavaScript
tags: AngularJs
published: true
---

A few tips and a few standards related to using the component pattern with AngularJs.  Highly suggsted to start writing your AngularJs project with this pattern in mind due to the migration path to AngularJs 2.0.

- Don’t use [ng-controllers](http://teropa.info/blog/2014/10/24/how-ive-improved-my-angular-apps-by-banning-ng-controller.html); instead modularize your code into directives.
- Reduce your reference to $scope.  Instead use ControllerAs with vm.
- Utilize the [PubSub pattern](http://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern); communicate between directives (components) with loosely coupled events.
- Keep AngularJs 2.0 in the back of your mind while writing your AngularJs apps. [http://youtu.be/uD6Okha_Yj0](http://youtu.be/uD6Okha_Yj0)
- For further Reference concerning these patterns, see the following [post](/sites/Engineering/Dev/blog/Lists/Posts/Post.aspx?List=7b352325-6321-4dc8-9309-c32888f5cae0&ID=205&Source=http://crossroads/sites/Engineering/Dev/blog/Lists/Posts/AllPosts.aspx).
