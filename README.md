# Yuggoth

<img src="https://raw.github.com/yogthos/yuggoth/master/logo.jpg" 
 style="margin-left:50px;"
 hspace="20"
 alt="Yuggoth logo" title="a strange dark orb" align="right" width="200" height="200"/>
 
>"Yuggoth... is a strange dark orb at the very rim of our solar system... 
>There are mighty cities on Yuggoth—great tiers of terraced towers built of black stone... 
>The sun shines there no brighter than a star, but the beings need no light. 
>They have other subtler senses, and put no windows in their great houses and temples..."

> — H. P. Lovecraft, &quot;The Whisperer in Darkness&quot;


Yuggoth is a blog engine which powers my site at http://yogthos.net   

## Features

* content caching
* RSS feed
* tags
* markdown in posts and comments with preview
* syntax highlighting using [syntax highlighter](http://alexgorbatchev.com/SyntaxHighlighter/)
* file uploads and management through web UI
* custom CSS styles
* captchas for comments
* latest comments view
* toggle post visibility
* localization

## Usage

The blog requires an instance of postgreSQL. On the first run the blog will guide you through setting up
the db connection properties and create the necessary tables for you. Then you will be presented with the 
setup wizard wich will allow you to configure the administrator and the blog title. Further configuration 
can be done on the profile page.   

If you use cake, substitute 'lein' with 'cake' below. Everything should work fine.
```bash
lein deps
lein run
```

to run as standalone
```bash
lein uberjar
java -jar yuggoth-0.4.0-SNAPSHOT-standalone.jar
```
Builds are available as a [jar](http://yogthos.net/files/yuggoth-0.4.0-SNAPSHOT-standalone.jar) for running
standalone and a [war](http://yogthos.net/files/yuggoth-0.4.0-SNAPSHOT-standalone.war) for app server deployment. 
 

valid options for running standalone

* -mode dev or prod
* -port integer

to make a deployable WAR
```bash
lein ring uberwar
```

see [markdown-clj](https://github.com/yogthos/markdown-clj) for supported syntax in posts, any valid HTML will work as well

 
## License

Distributed under the Eclipse Public License, the same as Clojure.

***
Copyright (C) 2012 Yogthos

