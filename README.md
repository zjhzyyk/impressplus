#Impressplus.js
A framework for easily creating Prezi-style presentation. [Check out the live demo](http://www.prism.gatech.edu/~yyang367/slide-demo/presentation.htm).

I get the idea from Impress.js. Impressplus.js is also based on CSS3 transforms and transition but is designed to offer more interactive features. With Impressplus.js, you can have a draggable and zoomable canvas not only in editing but also in presentation. 

The code is completely library agnostic: No jQuery, Prototype or similar is required.

I made an online graphical presentation authoring tool based on Impressplus.js. The website is at http://www.prism.gatech.edu/~yyang367/slidegen.html

##Instruction
1. All slide nodes should be in class "pslide" and be children of a parent node with id "presentation"
2. Impressplus.js constructs slides based on original CSS style of each slide node and slide order is determined by the order of node in DOM.

###Initialization
```javascript
prezi.init();
```
###Presentation
By default, in presentation, you are able to use following keys, left, right, space, and enter, to switch between slide. The side bar contains three four buttons. The home button is used to preview all slides in one screen. Zoomin and Zoomout buttons are used to zoom the canvas. Lock button is used to lock the canvas so that you can drag or zoom the canvas.

###Configuration
```javascript
prezi.init({
  sidebar: true, //whether show the sidebar
  mousewheel: true, //whether allow to use mousewheel to zoom the canvas
  slideClick: true //whether allow to change to another slide by clicking on the slide
});
```

##Development
####Minimization
```
$ npm install
$ grunt
```

