Blitter.js
==========

Description
-----------

Blitter.js lets you play sprite sheet animations. The class creates a `<canvas>` tag or a `<div>` tag depending 
on browser support.

Usage
-----

It's as easy as including the blitter.js file. No dependencies.

    var blitter = new Blitter({
        resource: "my/image.png",
        width: 40,
        height: 40,
        autoplay: false,  // default is true
        frameRate: 40,    // default is 30
        target: null      // if an existing dom element should be used
    });

    
    document.body.appendChild( blitter.getContainer() );
    
API
---

    var blitter = new Blitter({...});
       
    blitter.play();
    blitter.stop();
    blitter.gotoAndPlay(frame);
    blitter.gotoAndStop(frame);
    blitter.getContainer();

