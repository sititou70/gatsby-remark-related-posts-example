---
title: Vue.js
date: "2021-01-02T00:00:00.000Z"
description: "Vue.js is an open-source model–view–viewmodel front end JavaScript framework for building user interfaces and single-page applications."
---

Vue.js (commonly referred to as Vue; pronounced /vjuː/, like "view"[4]) is an open-source model–view–viewmodel front end JavaScript framework for building user interfaces and single-page applications.[11] It was created by Evan You, and is maintained by him and the rest of the active core team members.[12]

Overview

Vue.js features an incrementally adaptable architecture that focuses on declarative rendering and component composition. The core library is focused on the view layer only.[13] Advanced features required for complex applications such as routing, state management and build tooling are offered via officially maintained supporting libraries and packages,[14] with Nuxt.js as one of the most popular solutions.[citation needed]

Vue.js lets you extend HTML with HTML attributes called directives.[15] The directives offer functionality to HTML applications, and come as either built-in or user defined directives.
History

Vue was created by Evan You after working for Google using AngularJS in a number of projects. He later summed up his thought process: "I figured, what if I could just extract the part that I really liked about Angular and build something really lightweight."[16] The first source code commit to the project was dated July 2013, and Vue was first released the following February, in 2014.
Features
Components

Vue components extend basic HTML elements to encapsulate reusable code. At a high level, components are custom elements to which the Vue's compiler attaches behavior. In Vue, a component is essentially a Vue instance with pre-defined options.[17] The code snippet below contains an example of a Vue component. The component presents a button and prints the number of times the button is clicked:

Templates

Vue uses an HTML-based template syntax that allows binding the rendered DOM to the underlying Vue instance's data. All Vue templates are valid HTML that can be parsed by specification-compliant browsers and HTML parsers. Vue compiles the templates into virtual DOM render functions. A virtual Document Object Model (or “DOM”) allows Vue to render components in its memory before updating the browser. Combined with the reactivity system, Vue is able to calculate the minimal number of components to re-render and apply the minimal amount of DOM manipulations when the app state changes.

Vue users can use template syntax or choose to directly write render functions using JSX.[18] Render functions allow application to be built from software components.[19]
Reactivity

Vue features a reactivity system that uses plain JavaScript objects and optimized re-rendering. Each component keeps track of its reactive dependencies during its render, so the system knows precisely when to re-render, and which components to re-render.[20]
