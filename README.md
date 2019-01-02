# FHIR Implementation Guide - Build & Publish Template
A "starter kit" for creating, building, and publishing a static website for your [HL7 FHIR Implementation Guides](https://www.hl7.org/fhir/implementationguide.html). 

More information on Implementation Guide usage, authoring, publishing, and tools can be found at the [HL7 Wiki](http://wiki.hl7.org/index.php?title=FHIR_Implementation_Guides). This tool runs **Jekyll** to create a static site that can be hosted on a web server.

## What is Jekyll?
>"Jekyll is a simple, blog-aware, static site generator perfect for personal, project, or organization sites. Think of it like a file-based CMS, without all the complexity. Jekyll takes your content, renders Markdown and Liquid templates, and spits out a complete, static website ready to be served by Apache, Nginx or another web server. Jekyll is the engine behind GitHub Pages, which you can use to host sites right from your GitHub repositories."
–[Jekyll](https://jekyllrb.com/)

## Requirements
* [Ruby](https://www.ruby-lang.org/en/)
* [Bundler](http://bundler.io/)
* [Jekyll](https://jekyllrb.com/)

## Getting started
* Edit the ``src/sample-ig.xml`` file as necessary
* Add/change any static site content as required (e.g. images)
* Add/change any FHIR specific content as required, e.g.:
    * Page Content (``src/pagecontent/``)
    * Resources (``src/resources/``)
    * Vocabulary (``src/vocabulary/``)
    * Examples (``src/examples``)

* Execute a build to compile the IG into a static site (``*.sh`` and ``*.bat`` files inlcuded for Windows and Linux distributions):
    * ``_genonce.*`` Will execute a build 
    * ``_genUpdatePublisher.*`` Will download the HL7 IG Publisher tool and then execute a build
    * ``_clean.*`` Will clean the ``src-generated/`` directory


### Thanks
Many thanks to the HL7 team and the "Genomics Reporting" implementation guide, on which a lot of this template is based.

https://github.com/HL7/genomics-reporting

