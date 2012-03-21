Simple Globe to put your own data with latitude/longitude

You can instanciate it like that:

    var canvas = document.getElementById("3DView");
    var options = {
       globeBackColor: "#333333FF",
       globeFrontColor: "#888888aa",
       globeLinesColor: "#000000FF"
    };

    var globe = new Globe(canvas,options);
    
    var clickCallback = function() {
       console.log("cliked on image");
    };

    globe.addImage(48.8566667, 2.3509871, yourImage);
    globe.addImage(58.8566667, 2.2509871, yourOtherImage, {}, clickCallback );

[ Test Me ](http://cedricpinson.github.com/globe/)
