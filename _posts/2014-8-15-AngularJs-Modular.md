---
published: true
layout: post
category: JavaScript
tags: AngularJs
title: AngularJs: Make things more modular
---






There is a great talk that Nicholas Zakas gave (former front-end engineer for Yahoo and contributor to YUI).  He talks about decoupling the front-end into a modular web application utilizing the event-driven architecture pattern.  Here is a great summary as to how AngularJs acts like a Scalable Application Architecture.
http://serebrov.github.io/html/2013-03-18-js-scalable-architecture.html

**We can take this approach and relate it to AngularJs:**
- Base Library - AngularJs's own jqLite implementation
- App Core - angular itself using Pub/Sub to communicate between components
- Sandbox - scope passed to the controller
- Module - AngularJs Directives

To give a quick synopsis of that talk, it is based around the event-driven pattern.  There is a JavaScript framework called scaleApp that utilizes this type of pattern.  They have a good architecture synopsis on Nicholas Zakas’s approach that you can quickly digest:  http://scaleapp.org/readme.html#architecture-overview && http://www.microsoft.com/en-GB/developers/articles/scalable-javascript-application-architecture.
![Event Driven Architecture]({{site.baseurl}}/_posts/2014-8-15-AngularJs-Modular.event-driven-architecture.png)

To wrap-up, if we can talk about AngularJs and how we engineer it within our own domain utilizing a event-driven component / module methodology, I feel it can enhance our judgment when making decisions about its implementation and complementary frameworks and tools.

###References:
- Nicholas Zakas Video: http://youtu.be/b5pFv9NB9fs
- Slides: http://www.slideshare.net/nzakas/scalable-javascript-application-architecture
- Scalable JavaScript Design Patterns: http://addyosmani.com/scalablejs/
- Martin Beeby: http://www.microsoft.com/en-GB/developers/articles/scalable-javascript-application-architecture
- Tanner Linsley builds modular Angular site: http://nozzle.io/devblog/relative-angularjs-modules/
- Component Pattern - don't use ng-controller: http://teropa.info/blog/2014/10/24/how-ive-improved-my-angular-apps-by-banning-ng-controller.html
