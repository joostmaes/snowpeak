---
layout: layouts/home.njk
title: Home
date: 2016-01-01T00:00:00.000Z
permalink: /
eleventyNavigation:
  key: Home
  order: 0
- label: 'Home Section'
  name: 'sections'
  widget: 'list'
  types:
    - label: 'Carousel'
      name: 'carousel'
      widget: object
      summary: '{{fields.header}}'
      fields:
        - { label: Header, name: header, widget: string, default: 'Image Gallery' }
        - { label: Template, name: template, widget: string, default: 'carousel.html' }
        - label: Images
          name: images
          widget: list
          field: { label: Image, name: image, widget: image }
    - label: 'Spotlight'
      name: 'spotlight'
      widget: object
      fields:
        - { label: Header, name: header, widget: string, default: 'Spotlight' }
        - { label: Template, name: template, widget: string, default: 'spotlight.html' }
        - { label: Text, name: text, widget: text, default: 'Hello World' }
---

# Welcome henkie hoi

This is a template for building a simple blog website with the [Eleventy static site generator](https://www.11ty.io), with deployment to [Netlify](https://www.netlify.com).

{{title}}

Includes [Netlify CMS](https://www.netlifycms.org) for WYSIWYG content editing, and [Netlify Forms](https://www.netlify.com/docs/form-handling) for processing your site's form data.

For more info on installation and usage, view the \[project repo]({{ pkg.repository.url }}) on GitHub.

Or click the button below to deploy your own copy of this project to Netlify.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/danurbanowicz/eleventy-netlify-boilerplate&stack=cms)
