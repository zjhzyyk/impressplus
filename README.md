This project is deprecated. Please go [https://github.com/zjhzyyk/slide-maker](https://github.com/zjhzyyk/slide-maker) for a new version of slide maker.

#Impressplus.js
A framework for easily creating Prezi-style presentation. 

I got the idea from Impress.js. Impressplus.js is based on CSS3 transforms and transition. What is different from Impress.js is that with Impressplus.js, you can interact with the canvas by dragging the canvas using your mouse or zooming the it using mouse wheel when you are editing or presenting, while in Impress.js 

The code is completely library agnostic: No jQuery, Prototype or similar is required.

##Instruction
1. All slide nodes should be in class "pslide" and be children of a parent node with id "presentation".
2. Impressplus.js constructs slides based on original CSS style of each slide node and slide order is determined by the order of node in DOM.
3. You can save slide to your computer by starting presentation and save the presentation page by your web browser. You should then get a HTML file and a folder that includes resources needed by the presentation. You are now able to open the presentation by web browser.

###Initialization
```javascript
prezi.init();
```
###Presentation
By default, in presentation, you are able to use following keys, left, right, and enter, to switch between slide. The side bar contains four buttons. The home button is used to preview all slides in one screen. Zoomin and Zoomout buttons are used to zoom the canvas. Lock button is used to lock the canvas so that you can drag or zoom the canvas.

###Configuration
```javascript
prezi.init({
  sidebar: true, //whether show the sidebar
  mousewheel: true, //whether allow to use mousewheel to zoom the canvas
  slideClick: true //whether allow to switch to another slide by clicking on it
});
```

###Compatibility
Impressplus.js supports Chrome, Safari, Firefox, Opera, IE 10.

##Development
####Minimization
```
$ npm install
$ grunt
```

