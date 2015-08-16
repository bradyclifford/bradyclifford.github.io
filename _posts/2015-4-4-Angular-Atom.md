---
published: true
layout: post
title: "AngularAtom: Component-based Organization Directory Structure"
category: JavaScript
tags: AngularJs
---


With the changes in AngularJs 2.0 coming down the pipe, many have started to prepare for the component-based pattern. 

Dmitri Moore has a great blog around the [AngularAtom](http://demisx.github.io/angularjs/atom/component-feature-based-organization/2014/12/13/angular-1-component-organization-4.html) proposed directory structure that addresses the component-based structure. Some of the takeaways for me pertaining to this article are I have summarized:

**Components folder**: all stateless components / services.
- A components folder can have sub components
  - A component has a component.model.js file and a component.service.js.  The model contains the data while the service is responsible for getting, setting that data.
  - Single responsibility per file standard.  Does not place controller, directive and module within the same file.
  - Component folder can contain a Data folder for specific JSON data files and related assets
- Each component or state folder can contain a i18n folder for resource localization
- **State folder**: contains everything necessary to render the particular UI state
  - Instead of placing all routes / states within a single route.js config file, they are modularized.  Each state folder contains its own route config file with that specific route / state.
  - Each state may contain one or more child states that, unlike sub-components, each define their own module.  This is because each state, be it parent or child, is looked at as an independent citizen that can be added or removed at any time of the application lifecycle.

```
1. 'phones'         // abstract state, can't be transitioned to
2. 'phones.list'    // UI shows a list of all phones
3. 'phones.detail'  // UI shows detail info on the selected phone
 
         |phones| // <-- abstract state that loads default layout
           /  \
          /    \
         /      \
      |list|  |detail| // <-- concete states that plug in their own content into the default layout
```
-** Layout folder**: contains all partial files that support the application shell. 
  - Layouts are injected into the main app/index.html by the abstract states. Your public section, for example, may inject one layout (ex. public.html) from the app.public abstract state, with this the secure section may inject a completely different layout (ex. secure.html) from the app.secure abstract state.
- **Helpers folder**: contains a collection of various utilities not specific to any component. Usually implemented as JS pure functions.

Summary of Dmitri Moore’s the folder structure below.  For a full view of the folder structure, see his [GitHub](https://gist.github.com/demisx/cbbf605db31e7c9f5cf6).

```
[app-name]/ # application root directory
  |__app/   # container for all user-generated app code
  |   |__components/   # stateless feature components
  |   |__layouts/      # layout specific partials
  |   |__states/       # application UI states
  |__vendor/ # 3rd party vendor client libraries global to the entire app
  |__config/           # app related configuration
  |__node_modules/     # 3rd party vendor node.js modules global to the entire app
  |__scripts/          # shell scripts like Glup tasks
  |__tests/            # e2e tests
```
[John Papa’s style guide](https://github.com/johnpapa/angular-styleguide#folders-by-feature-structure) is similar to what the [AngularAtom](https://gist.github.com/demisx/cbbf605db31e7c9f5cf6) folder structure is suggesting; just isn’t as detailed.
- Folder by Feature: create folders named for the feature they represent. When a folder grows to contain more than 7 files, consider creating a new folder.
- Layout Folder: components that define the overall layout of the application; these may include a shell view and controller (navigation, menus, etc.)
