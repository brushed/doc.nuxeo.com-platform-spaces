---
title: Nuxeo JSF UI
review:
    comment: ''
    date: '2015-12-01'
    status: ok
labels:
    - jsf
    - todo
    - seam-jsf-component
    - multiexcerpt-include
    - excerpt
tabbed_page: true
toc: true
confluence:
    ajs-parent-page-id: '16089312'
    ajs-parent-page-title: JSF UI Framework
    ajs-space-key: NXDOC
    ajs-space-name: Nuxeo Platform Developer Documentation
    canonical: Nuxeo+JSF+UI
    canonical_source: 'https://doc.nuxeo.com/display/NXDOC/Nuxeo+JSF+UI'
    page_id: '950313'
    shortlink: KYAO
    shortlink_source: 'https://doc.nuxeo.com/x/KYAO'
    source_link: /display/NXDOC/Nuxeo+JSF+UI
tree_item_index: 100
history:
    -
        author: Manon Lumeau
        date: '2016-09-27 12:54'
        message: ''
        version: '26'
    -
        author: Manon Lumeau
        date: '2016-09-26 16:11'
        message: ''
        version: '25'
    -
        author: Solen Guitter
        date: '2016-09-05 09:37'
        message: ''
        version: '24'
    -
        author: Manon Lumeau
        date: '2016-07-20 13:42'
        message: remove children display macro
        version: '23'
    -
        author: Solen Guitter
        date: '2015-12-14 15:03'
        message: ''
        version: '22'
    -
        author: Solen Guitter
        date: '2015-08-31 14:07'
        message: Update table of contents look
        version: '21'
    -
        author: Anahide Tchertchian
        date: '2014-12-09 13:42'
        message: 'NXDOC-427: add sub pages index'
        version: '20'
    -
        author: Anahide Tchertchian
        date: '2014-12-01 18:25'
        message: ''
        version: '19'
    -
        author: Anahide Tchertchian
        date: '2014-12-01 18:24'
        message: 'NXDOC-196: remove warning'
        version: '18'
    -
        author: Anahide Tchertchian
        date: '2014-12-01 18:24'
        message: 'NXDOC-196: review content'
        version: '17'
    -
        author: Alain Escaffre
        date: '2014-11-24 16:53'
        message: ''
        version: '16'
    -
        author: Gildas Lefevre
        date: '2014-11-04 17:46'
        message: Update versions of technical stack
        version: '15'
    -
        author: Alain Escaffre
        date: '2014-01-10 18:14'
        message: ''
        version: '14'
    -
        author: Alain Escaffre
        date: '2014-01-10 18:14'
        message: ''
        version: '13'
    -
        author: Solen Guitter
        date: '2014-01-07 14:57'
        message: ''
        version: '12'
    -
        author: Anahide Tchertchian
        date: '2013-12-20 15:05'
        message: ''
        version: '11'
    -
        author: Anahide Tchertchian
        date: '2013-12-04 17:26'
        message: add WIP warning
        version: '10'
    -
        author: Anahide Tchertchian
        date: '2013-12-04 13:46'
        message: Reverted from v. 7
        version: '9'
    -
        author: Anahide Tchertchian
        date: '2013-12-04 13:44'
        message: remove JSF stack part (moved to sub page)
        version: '8'
    -
        author: Anahide Tchertchian
        date: '2013-12-04 12:39'
        message: ''
        version: '7'
    -
        author: Solen Guitter
        date: '2013-09-05 15:44'
        message: Added TOC
        version: '6'
    -
        author: Solen Guitter
        date: '2011-03-04 10:46'
        message: Migrated to Confluence 4.0
        version: '5'
    -
        author: Solen Guitter
        date: '2011-03-04 10:46'
        message: ''
        version: '4'
    -
        author: Solen Guitter
        date: '2011-03-04 10:46'
        message: formatting and typos
        version: '3'
    -
        author: Thierry Delprat
        date: '2010-10-15 01:01'
        message: ''
        version: '2'
    -
        author: Admin name placeholder
        date: '2010-03-01 01:35'
        message: ''
        version: '1'

---
# Functional Overview

## &nbsp;Nuxeo Platform Concepts

{{{multiexcerpt 'functional-overview' page='USERDOC:Nuxeo Platform Concepts'}}}

## Creating Content

{{{multiexcerpt 'functional_overview' page='USERDOC:Creating Content'}}}

## Editing Content

### Content and Metadata Edit Form

{{{multiexcerpt 'edit-document' page='USERDOC:Editing Content'}}}

{{{multiexcerpt 'edit-form-custom-functional-overview' page='USERDOC:Editing Content'}}}

### Clipboard and Worklist

{{{multiexcerpt 'clipboard-worklist-overview' page='USERDOC:Editing Content'}}}

# Technical Overview

{{! excerpt}}

The Nuxeo Platform provides a web framework to build business applications for thin clients. This framework is based on the standard JEE view technology: Java Server Faces (JSF).

{{! /excerpt}}

## Nuxeo JSF Technical Stack

Nuxeo JSF framework integrates several technologies in order to make the development of web applications fast and efficient.

The Nuxeo JSF stack includes:

*   Mojarra JSF (2.2.6) as MVC and UI component model, including, as of JSF 2 specifications, facelets as rendering engine and templating system,
*   RichFaces (4.5.0) for high level UI components, including the a4j library for Ajax behaviors support
*   JBoss Seam (2.3.1) as Web Framework

Inside the Nuxeo Platform, Seam Framework is used only for the JSF (client) layer.

The usage of Seam has several benefits:

*   usage of JSF is simpler,
*   powerful context management,
*   dependency injection and Nuxeo Service lookup via injection,
*   Nuxeo Web Component are easily overridable,
*   decoupling of Web Components (that can communicate via Seam event bus).

The Nuxeo JSF framework also comes with additional concepts and tools:

*   [Action service]({{page page='actions-links-buttons-icons-tabs-and-more'}}) is used to make buttons, tabs and views configurable.
*   [Layout]({{page page='layouts-and-widgets-forms-listings-grids'}}) and [Content View]({{page page='content-views'}}) allow to define how you want to see documents and listings.
*   [URL Service]({{page page='navigation-urls'}}): the Nuxeo Platform provides REST URLs for all pages so that you can bookmark pages or send via email a link to a specific view on a specific document.
*   [Nuxeo Tag Libraries]({{page page='how-to-register-a-jsf-tag-library'}}): extend existing tags and provides new Document Oriented tags.
*   [Theme engine]({{page page='theme'}}).

## Nuxeo JSF Approach

We built Nuxeo JSF framework with two main ideas in mind:

*   Make the UI simple,
*   Make the UI pluggable.

For the first point, we choose to have an "File Explorer" like navigation. So you have tools (tree, breadcrumb, search, tags) to navigate in a document repository and when on a document you can see several views on this document (Summary, Relations, Workflows, Rights, History ...).

We also choose to make the UI very pluggable, because each project needs to have a slightly different UI. In order to achieve that, each page/view is in fact made of several fragments that are assembled based on the context. This means you can easily add, remove or change a button, a link, a tab or a HTML/JSF block. You don't need to change or override the Nuxeo Platform code for that, neither do you need to change the default Nuxeo Platform templates. The assembly of the fragments is governed by "Actions", so you can change the filters and conditions for each fragment. Of course each project also needs to define it's own views on Document, for that we use the Layout and Content View system.

All this means that you can start from a standard Nuxeo Platform, and with simple configuration have a custom UI.

## Pages Index

*   [JSF Page Layout System Overview]({{page space='NXDOC' page='JSF Page+Layout+System+Overview'}})
*   [Web UI Limitations]({{page space='NXDOC' page='Web UI+Limitations'}})&nbsp;&mdash;&nbsp;<span class="smalltext">This chapter presents the limitations to the Seam/JSF web application.</span>
*   [Web UI How-To Index]({{page space='NXDOC' page='Web UI+How-To+Index'}})
*   [Upgrade to JSF2]({{page space='NXDOC' page='Upgrade to+JSF2'}})&nbsp;&mdash;&nbsp;<span class="smalltext">The Nuxeo Platform has been upgraded to JSF 2 for the 6.0 version. This page provides tools and notes to help you migrate your custom Nuxeo projects to this version.</span>
*   [JSF and Ajax Tips and How-To Index]({{page space='NXDOC' page='JSF and+Ajax+Tips+and+How-To+Index'}})

# Installation & Configuration

## Installation

### Installing Nuxeo JSF UI Addon &nbsp;

{{{multiexcerpt 'MP-installation-easy' page='Generic Multi-Excerpts'}}}

Once the addon is installed, you can go to [https://host:port/nuxeo](https://hostport) and after authentication, you will be able to browse the JSF UI and start creating content, upload files, browse and search for content.

## Configuration

### Configuring Nuxeo JSF UI Addon

There is no additional configuration step required to start using the addon. Customisation is done via Nuxeo Studio.

{{> end_of_tabs }}
