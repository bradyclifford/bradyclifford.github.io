---
published: true
layout: post
title: Building our JavaScript
category: JavaScript
---


I attempted to convince the architecture committee at one of my jobs why we needed to build our JavaScript.  I put together a [slidedeck](http://www.slideshare.net/bradyclifford/building-javascript) that went through the whys and the benefits.  [Take a look](http://www.slideshare.net/bradyclifford/building-javascript)...

I based my slidedeck on the presentation [Peter Hunt](https://youtu.be/VkTCL6Nqm6Y) gave back in 2014.  **To summarize:**
- Spas are the best UX experience
- Con is that the initial load takes too long
- Instagram has 10 SPAs in their architecture
- Reduce amount of HTTP requests & bytes downloaded
- Bundling everything into one file is not the best approach2.5MB gzip bundled file is too big.
- Utilize a module system to intelligently bundle your packages with a dynamic dependency map.

The 2 slides from his presentation that impacted me the most:
![Bundled Modules Example]({{site.baseurl}}/images/posts/2015-05-7-Build-JavaScript.bundled-modules.png)
![Optimized Bundled Modules Example]({{site.baseurl}}/images/posts/2015-05-7-Build-JavaScript.optimized-bundles.png)

###Overall, I arguired the need to build web front end code so one could:
- **Developers to mimic production on their own box**.
  - Developers are able to identify concatenation and minification issues before code is checked in.
  - The build config is shared amongst all environments
Prepares us for AngularJs 2 and ES6

- **Automated versioning of shared packaged libraries**.
  - Treat our shared libriaries like 3rd parties
  - On check-in, build, package and version shared libraries deploying to local package repository like git.  This speeds up the build process for the Spa and also removes versioning within TFS.
  
  - Part of the build process can also incorporate the automation of generating documentation and demos.  See how AngularStrap and UI-Boostrap and achieving this from their source code.

- **Utilize a package manager and a local rev. repository**.
- **Automated builds of documentation and shared component demos**.
- **Reduction and even elimination of Glofs and Glogs**.

- **Reduce initial Spa loading time** through intelligent bundling: use a module system and an intelligent dependency map bundling tool, like webpack.

- **Architecting our web application code so it is web server agnostic**.
  - Instead of loading 100+ servers with our web application files, we can upload them to one location
  - Avoids the second hop to our F5 and web farm in our current architecture
  - Brings us closer to a true micro services SOA architecture; separating the front end from the middle tier.
  - Allows us to use redirection only for api calls.  Don’t have to perform a browser redirect during login.
  - An example of a server agnostic web application:
  ![2015-05-7-Build-JavaScript,objective-6.png]({{site.baseurl}}/images/posts/2015-05-7-Build-JavaScript,objective-6.png)

