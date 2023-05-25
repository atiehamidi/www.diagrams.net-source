---
title: Step through your diagram using the explore plugin
layout: page
faq: true
categories: [Plugins]
---

_This plugin should be used as-is, as an unsupported example for developers._

The explore plugin allows you to step through your diagram from the point of view of a shape (or a node) in your diagram. When you explore from a shape, you can click on the paths away from and to that shape, without the distraction of the rest of your potentially complex diagram.

This is useful for exploring complex organisation charts, mind maps, UML class diagrams, flow charts and more.

[More information about draw.io plugins](/doc/faq/plugins.html)

## Load the explore plugin

* To create a new diagram in our online editor with the plugin already loaded, go to [https://app.diagrams.net/?splash=0&p=ex](https://app.diagrams.net/?splash=0&p=ex)

## Explore a diagram

Once you have loaded the explore plugin, right click on a shape to see the context menu, and select _Explore from here_, which should be at the bottom of the menu.

This will open your diagram in the lightbox, showing on the shape you selected and its connected shapes.

<img src="/assets/img/blog/explore-from-here.gif" style="max-width:100%;height:auto;" alt="Using the explore plugin to step through a complex org chart">

## Permanently load the plugin

If you want to always be able to explore your diagrams like this, add the explore plugin to the plugins list to load it each time you create or edit a diagram.

1. From the menu, select _Extras > Plugins_.
<br /><img src="/assets/img/blog/extras-plugins.png" style="width=100%;max-width:400px;height:auto;" alt="Open the plugins list">
2. Click _Add_.
<br /><img src="/assets/img/blog/add-plugin.png"style="width=100%;max-width:200px;height:auto;" alt="Add a new plugin">
3. Select ``ex`` in the drop-down list of built-in plugins, then click _OK_.
<br /><img src="/assets/img/blog/add-explore-plugin.png" style="width=100%;max-width:200px;height:auto;" alt="Add the explore plugin">
4. Click _Apply_.
<br /><img src="/assets/img/blog/apply-add-explore-plugin.png" style="width=100%;max-width:200px;height:auto;" alt="Add the explore plugin">

Reload your browser tab to load the plugin into the diagram editor.

## Share a diagram so it can be explored

By default, diagrams published to URLs do not load plugins.

To allow someone to explore your diagram, when you publish a diagram to a URL (_File > Publish Link_), add the ``&p=ex`` URL parameter to the link before you share it (as highlighted in blue in the screenshot below).

<img src="/assets/img/blog/share-link-explore-plugin.png" style="width=100%;max-width:400px;height:auto;" alt="Share a link to your diagram and enable the explore plugin">

**Note:** Plugins are not supported in draw.io for Confluence.
