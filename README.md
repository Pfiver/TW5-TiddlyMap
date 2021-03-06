TiddlyMap
=====================================================================

TiddlyMap is a TiddlyWiki plugin that allows you to link your wiki-topics (tiddlers) in order to create *clickable graphs*. By creating relations between your topics you can easily do the following:

* **Create mindmaps** and quickly manifest your ideas in tiddlers (wiki entries).
* **Create task-dependency graphs** to organize and describe your tasks.
* **Visualize your topic structures** to get an immediate grasp of topics and relations.

In general you may create, visualize and describe any network-structure you have in mind.

A demo with several examples and explanations can be found [here](http://bit.ly/tiddlymap).

How it works
---------------------------------------------------------------------

TiddlyMap combines the strength of two open-source projects.

#### The TiddlyWiki Project

> [TiddlyWiki](http://tiddlywiki.com/) has bought unprecedented freedom to people to keep their precious information under their own control.
> – [tiddlywiki.com]([http://tiddlywiki.com]/#TiddlyWiki)

The TiddlyWiki project is a flourishing community project under the lead of its original inventor Jeremy Ruston. Put in simple words, TiddlyWiki is a highly interactive wiki stored in a single file that can be used for:

* Personal note taking
* Project documentation and management
* To create whole encyclopedias

The building blocks of TiddlyWiki are small pieces of information called "tiddlers":

> "Tiddlers" are fundamental units of information. Tiddlers work best when they are as small as possible so that they can be reused by weaving them together in different ways. The TiddlyWiki project aspires to provide a concise way of expressing and exploring the relationships between these small pieces of information.
> –  Adapted from [Philosophy of Tiddlers](http://tiddlywiki.com/#Philosophy%20of%20Tiddlers) and [Tiddlers](http://tiddlywiki.com/#
Tiddlers)

#### The Vis.js Project

For graph visualization and manipulation, TiddlyMap draws upon the popular open-source [vis.js](http://visjs.org/) library - *a dynamic, browser based visualization library* actively developed and maintained by a team of enthusiastic developers working at [Almende B.V](|http://almende.com).

> The library is designed to be easy to use, handle large amounts of dynamic data, and enable manipulation of the data
> – [visjs.org](|http://visjs.org/)

Impressions
---------------------------------------------------------------------

#### :paperclip: Use colors and icons in your graphs

![tiddlymap demo site create clickable graphs and mindmaps by simply linking your tiddlers - chromium_439](https://cloud.githubusercontent.com/assets/4307137/5756039/85fc17ba-9cab-11e4-914e-e2176af1af15.png)

#### :paperclip: Work fullscreen

![tiddlymap demo site create clickable graphs and mindmaps by simply linking your tiddlers - chromium_443](https://cloud.githubusercontent.com/assets/4307137/5755990/09d15308-9cab-11e4-8bf0-d9bd6c5a0c4f.png)

#### :paperclip: Use filters to decide what nodes to display in the graph

![tiddlymap demo site create clickable graphs and mindmaps by simply linking your tiddlers - chromium_444](https://cloud.githubusercontent.com/assets/4307137/5756086/317535c2-9cac-11e4-99e6-6f048f512e6b.png)

#### :paperclip: Get search results as graph (including direct neighbours)

![tiddlymap demo site create clickable graphs and mindmaps by simply linking your tiddlers - chromium_441](https://cloud.githubusercontent.com/assets/4307137/5756022/60369244-9cab-11e4-880a-41ca63663c89.png)

#### :paperclip: Create hierarchical layouts based on certain edge types

![tiddlymap demo site create clickable graphs and mindmaps by simply linking your tiddlers - chromium_445](https://cloud.githubusercontent.com/assets/4307137/5756112/7966e902-9cac-11e4-838c-788393843814.png)

Installation
---------------------------------------------------------------------

By using this plugin you agree to the product's [License Terms](https://github.com/felixhayashi/TW5-TiddlyMap/blob/master/LICENSE) (TiddlyMap is distributed under the [BSD 2-Clause License](http://opensource.org/licenses/BSD-2-Clause)).

#### When running in Nodejs

For general information on how to set up TiddlyWiki5 with Nodejs visit [tiddlywiki.com](http://tiddlywiki.com). The instructions here are for installing plugins on the node.js server.  This way, the same plugin can be served to many TiddlyWikis.  Multiple wikis will all use the same plugin instance.  You can also install via the standard drag-and-drop method (see below) in a single wiki being served on node.js, but the plugin will only be installed for that wiki.  The process, including all updates, will have to be repeated for all other wikis if you plan on serving more than one.

1. Download a copy of the following plugins: [TiddlyMap](https://github.com/felixhayashi/TW5-TiddlyMap), [TW5-TopStoryView](https://github.com/felixhayashi/TW5-TopStoryView),[TW5-Vis.js](https://github.com/felixhayashi/TW5-Vis.js)
    * by either cloning each repository.
    * or by clicking "Download ZIP" and unzipping it.
2. For each plugin, Copy the folder that resides directly below `dist/felixhayashi/` and move it into the `TiddlyWiki5/plugins/` folder (varies with OS.  Linux: "/usr/lib/node_modules/tiddlywiki/plugins").
3. Update the plugin section of your wiki's `tddlywiki.info` file (resides in the root of your wiki) to contain the following:

        {
          "plugins": [
            
            ...
            
            "felixhayashi/topstoryview",
            "felixhayashi/vis",
            "felixhayashi/tiddlymap",
            
            ...
            
          ]
        }
4. Restart your wiki server via the command line
5. If you want to use the "live view", change your wiki's story view to "Top" (Configuration ➡ Appearance ➡ Story view ➡ Current view).

#### Standalone

Please follow the instructions given [here](http://felixhayashi.github.io/TW5-TiddlyMap/index.html#How%20to%20install%20TiddlyMap%3F)
