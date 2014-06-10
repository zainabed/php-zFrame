php-zFrame
==========

PHP MVC Framework

Lightweight PHP Framework which follows MVC pattern

Installation
------------

git clone https://github.com/zainabed/php-zFrame
and update httpd.conf settings as

<pre><code>
&lt;VirtualHost *:8081&gt;
    ServerName domain_name
    DocumentRoot "path of cloned repository"
    DirectoryIndex index.php

    &lt;Directory " path of cloned repository "&gt;
        AllowOverride All
	Allow from All
    &lt;/Directory&gt;
&lt;/VirtualHost&gt;
</code></pre>

Directory Structure
-------------------

-  App
  -  Module (Module name e.g Demo
		-  Block ( Independent Partials e.g Sidebars, Ajax Controller, JSON REST API )
		-  Config ( Module Routing, Asset {View, Layout, Skin} configurations 
		-  Controller 
		-  Layout (Module based Layout files)
		-  Model (Module based Model Classes)
		-  View (Module based Views)
  -  Cache
	  -  Routing Cache (At the moment)
  -  Config
	  -  Application, Module, Database Configurations
  -  Lib
	  -  Application Related Libraries ( Base Controller, Base Block, Routing, Http, View )
  -  Skin
	  -  Javascript, CSS files
  -  Web
	  -  Other global access PHP files
