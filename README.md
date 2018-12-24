# Uix Kit


[![Travis CI](https://api.travis-ci.org/xizon/uix-kit.svg?branch=master)](https://travis-ci.org/xizon/uix-kit/)
[![npm version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=js&type=6&v=3.0.0&x2=0)](https://www.npmjs.com/package/uix-kit)
[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE)


<p align = "left">
    <img width="300" src="https://uiux.cc/uix-kit/assets/images/logo-colorful.png">
</p>

---


[Demo](https://uiux.cc/uix-kit) | [NPM](https://www.npmjs.com/package/uix-kit)



## Table of Contents


* [Getting Started](#getting-started)
* [Description](#description)
* [Installation And Test](#installation-and-test)
* [How To Use？](#how-to-use)
* [Contributing](#contributing)
* [Changelog](#changelog)
* [Browser Support](#browser-support)
* [Licensing](#licensing)
* [Buy Me a Coffee](#buy-me-a-coffee)



## Getting Started


<p align = "left">
	<a href="https://www.youtube.com/watch?v=ckYJBMfPtBs"><img src="https://uiux.cc/uix-kit/misc/screenshots/video-cover.jpg" width="400"></a>
</p>



## Description

Make over <strong>120+</strong> components to wear again and again!


An underlying front-end system that makes it easy to extend and modify core files. This spec is a living document that will be updated as we continue to develop the tenets and specifics of Uix Kit. Support JS, HTML and SASS component library automatically packaged. Automatically convert ES6 JS to ES5 using Babel in this scaffold.

Enjoy the fluid grid system based on Bootstrap and self-expansion. Uix Kit is built over Bootstrap and has all the benefits that the framework comes with. Regardless of the screen size, the website content will naturally fit the given resolution. Using the Uix Kit will save you large amount of time to build your projects. It supports 3D and 2D rendering with three.js and pixi.js. More typically, automatically generate core files with Webpack for each module (contains .js, .scss, .html files).

* Supports 3D and 2D rendering with three.js and pixi.js.
* Using Sass to Control Scope With BEM Naming
* Automatically generate table of contents for each module comment of name.
* Simple custom CSS and JS core files
* 100% Responsive & Mobile Ready
* Prepare some generic plug-ins in advance
* Core style sheet compatible with Bootstrap 4.x
* Provides a common web page components and layouts
* W3C Standard Support
* Support PJAX no refresh method for loading pages
* Support JS, HTML and SASS component library automatically packaged.
* Make a foundation for the React architecture.


* * *


## Installation And Test

**Step 1.** Use NPM (Locate your current directory of project, and enter the following command.) or download the latest version from [Github](https://github.com/xizon/uix-kit). For nodejs you have to install some dependencies.

```sh
$ sudo npm install uix-kit
```

Or clone the repo to get all source files including build scripts: 

```sh
$ git clone git://github.com/xizon/uix-kit.git
```


**Step 2.** First, using an absolute path into your `"uix-kit/"` folder directory.

```sh
$ cd /{your_directory}/uix-kit
```


**Step 3.** Before doing all dev stuff make sure you have `Node 10+` installed. After that, run the following code in the main directory to install the node module dependencies.

```sh
$ sudo npm install --save-dev  --unsafe-perm node-sass
```


**Step 4.** Run the following code to enter development mode. The converted ES5 files will be created.

```sh
$ npm run build
```

**Step 5.** When you done, please open the browser and enter the following URL to check out.

```sh
http://localhost:8080/examples/
```


### Note:
 
**ERROR: npm update check failed.**

```sh
$ sudo chown -R $USER:$(id -gn $USER) /Users/{username}/.config
```



* * *


## How To Use

### 1\. HTML Structure

```html

<!DOCTYPE html>
<html dir="ltr" lang="en-US">
	<head>
		<meta charset="utf-8" />
		<title></title>	
        
		<!-- Mobile Settings
		============================================= -->
        <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1" />
        <!-- Mobile Settings end -->
        
		<!-- Core library
		============================================= -->
		<script src="assets/js/wp-jquery/jquery.min.js?ver=2.1.3"></script>
		<script src="assets/js/wp-jquery/jquery.migrate.min.js?ver=1.4.1"></script>
		<script src="assets/js/min/prefixfree.min.js?ver=1.0.7"></script>
		<!-- Core library  end -->
		
		
		<!-- Compatibility
		============================================= -->
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        
        <script src="assets/js/min/modernizr.min.js?ver=3.5.0"></script>
        
        <!--[if lt IE 9]>
            <script src="assets/js/min/respond.min.js?ver=1.4.2"></script>
        <![endif]-->
        
        <!-- Compatibility  end -->



		<!-- Core & Theme CSS
		============================================= -->
        
        <!-- Basic  -->
        <link rel="stylesheet" href="assets/css/bootstrap.min.css?ver=4.1.3" media="all"/>
		<link rel="stylesheet" href="assets/css/video.min.css?ver=5.19" media="all"/>
		
        <!-- Icons  -->
        <link rel="stylesheet" href="assets/fonts/fontawesome/font-awesome.min.css?ver=4.5" media="all" />  
        
        <!-- Theme  -->
        <link rel="stylesheet" href="../dist/uix-kit.min.css?ver=1.0.0" media="all"/>
        
     
         <!--[if lt IE 10]>
           <link rel="stylesheet" href="../dist/uix-kit.IE.css?ver=1.0.0" media="all" />
        <![endif]-->
        
        
        <!-- Core & Theme CSS  end -->
        
     
  </head>     
  <body>
  
  
          
    ...

  

    <!-- Basic Script -->
	<script src="assets/js/min/jquery.easing.min.js?ver=1.3"></script>
    <script src="assets/js/min/jquery.waitforimages.min.js?ver=1.0"></script>
    <script src="assets/js/min/video.min.js?ver=5.19"></script> 
	<script src="assets/js/min/jquery.waypoints.min.js?ver=4.0.1"></script> 
    <script src="assets/js/min/template7.min.js?ver=1.2.5"></script>
    <script src="assets/js/min/TweenMax.min.js?ver=1.20.4"></script>
    <script src="assets/js/min/pixi.min.js?ver=4.7.1"></script>
    <script src="assets/js/min/three.min.js?ver=r92"></script>
    <script src="assets/js/min/anime.min.js?ver=2.2.0"></script>
    <script src="assets/js/min/hammer.min.js?ver=2.0.8"></script>
    
    <!-- Masonry -->
    <script src="assets/js/wp-jquery/masonry.min.js?ver=3.3.2"></script>
    <script src="assets/js/wp-jquery/imagesloaded.min.js?ver=4.1.0"></script>

    <!-- Filterable  -->
    <script src="assets/js/min/jquery.shuffle.min.js?ver=3.1.1"></script> 
    
    
	
	<!-- Your Plugins & Theme Scripts
	============================================= -->

	<script>
		var REVISION     = "1.0.0",
			APP_ROOTPATH = {
				"templateUrl" : "", //If the file is in the root directory, you can leave it empty. If in another directory, you can write: "/blog"
				"homeUrl"     : "",  //Eg. https://uiux.cc
				"ajaxUrl"     : ""   //Eg. https://uiux.cc/wp-admin/admin-ajax.php
			};
    </script>  
    <script src="../dist/uix-kit.min.js?ver=1.0.0"></script>


  </body>
</html>



```


### 2\. File Structures


```sh

uix-kit/
├── README.md
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── webpack.config.js
├── package-lock.json
├── package.json
├── dist/
├── misc/
│   ├── screenshots/
│   └── grid/
├── src/
│   ├── index.js
│   ├── index-rtl.js
│   ├── components/
│   │       ├── _global/
│   │       ├── _home/
│   │       └── ...
├── examples/
│   ├── *.html
│   ├── assets/
│   │       ├── css/
│   │       ├── fonts/
│   │       ├── images/
│   │       ├── videos/
│   │       ├── models/
│   │       ├── json/
│   │       └── js/
└──
```


### 3\. PSD Grid Templates

You can download the corresponding .PSD grid files based on Bootstrap 3.x from the `_grid` folder.

*   `misc/grid/bootstrap3_1170_grid_web.psd` (Default Container: 1170px)
*   `misc/grid/bootstrap3_1278_grid_web.psd` (XL Container: 1278px)
*   `misc/grid/bootstrap3_1410_grid_web.psd` (XXL Container: 1410px)



## Contributing

Finding bugs, sending pull requests or improving our docs - any contribution is welcome and highly appreciated. To get started, head over to our [contribution guidelines](CONTRIBUTING.md). Thanks!


## Changelog

[releases](CHANGELOG.md)



## Browser Support

![Chrome](https://raw.github.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png) | ![Firefox](https://raw.github.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png) | ![Edge](https://raw.github.com/alrra/browser-logos/master/src/edge/edge_48x48.png) | ![IE](https://raw.github.com/alrra/browser-logos/master/src/archive/internet-explorer_9-11/internet-explorer_9-11_48x48.png) | ![Safari](https://raw.github.com/alrra/browser-logos/master/src/safari/safari_48x48.png) | ![Opera](https://raw.github.com/alrra/browser-logos/master/src/opera/opera_48x48.png) | iOS  | Android
--- | --- | --- | --- | --- | --- | --- | --- |
45+ ✔ | 38+ ✔ | 12+ ✔ | 9+ ✔ | 9.1+ ✔ | 30+ ✔ | 10+ ✔ | 4.4+ ✔ |



## Licensing

Licensed under the [MIT](https://opensource.org/licenses/MIT).



## Buy Me a Coffee
Donations would be more than welcome :)

[![Donate](https://www.paypalobjects.com/en_US/GB/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=PYZLU7UZNQ6CE)

