---
layout: post
title: Multipage React Application
category: React

excerpt: My personal learnings on working with react modules on a cms generated website.

---

# Multipage React Application

**Setup:**
* node: 7.4.0
* react: 15.4.2
* webpack: 2.2.0

The problem was: We needed react functions inside a CMS based website. So the content has to come from the CMS database and the listing and filtering of products should come from an api and built via react.

Usual PHP CMS websites works with multiple physical sites.

React, especially with **Redux** and **Router** is built for singlepage applications with one physical site a virtual DOM and a common state.


## First approach
My first approach was to make the components of the application standalone. Without a Router and with all dependencies in each component. I would save the state in sessionStorage to communicate between the components.

### Fails:
I was working with Webpack. For multiple components on one site you need multiple entry-points. See here: [https://webpack.js.org/concepts/entry-points/#multi-page-application](https://webpack.js.org/concepts/entry-points/#multi-page-application)
The problem with this entry points is that I would have to define entry points for each page (which will be generated dynamically via the CMS).

## Second approach
I will built a normal singlepage react application, grab the content from a cms generated site and paste it into the application.



