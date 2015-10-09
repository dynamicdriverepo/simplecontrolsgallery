# Simple Controls Gallery #

*Description:* Want to display images as an automatic slideshow that can also be explicitly played or paused by the user? Simple Controls Gallery rotates and displays an image by fading it into view over the previous one, with navigation controls that pop up when the mouse rolls over the Gallery. 

## Directions ##

*Step 1:* This script uses the following external files:

+ jQuery 1.6 or above (served via Google CDN)
+ simplegallery.js
+ simplegallery.css
+ jquery.touchSwipe.min.js
+ 5 images

*Step 2:* Add the below code to the HEAD section of your page:

	<link rel="stylesheet" href="simplegallery.css" />
	<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
	<script src="jquery.touchSwipe.min.js"></script>
	
	<script type="text/javascript" src="simplegallery.js">
	
	/***********************************************
	* Simple Controls Gallery- (c) Dynamic Drive DHTML code library (www.dynamicdrive.com)
	* Please keep this notice intact
	* Visit Dynamic Drive at http://www.dynamicdrive.com/ for this script and 100s more
	***********************************************/
	
	</script>
	
	<script type="text/javascript">
	
	var mygallery=new simpleGallery({
		wrapperid: "simplegallery1", //ID of main gallery container,
		dimensions: [250, 180], //width/height of gallery in [pixels, pixels] or ['percentage%', pixels]
		imagearray: [
			["http://dynamicdrive.com/dynamicindex4/pool.jpg", "http://en.wikipedia.org/wiki/Swimming_pool", "_new", ""],
			["http://dynamicdrive.com/dynamicindex4/cave.jpg", "http://en.wikipedia.org/wiki/Cave", "", ""],
			["http://dynamicdrive.com/dynamicindex4/fruits.jpg", "", "", ""],
			["http://dynamicdrive.com/dynamicindex4/autumn.jpg", "", "", ""]
		],
		autoplay: [true, 2500, 2], //[auto_play_boolean, delay_btw_slide_millisec, cycles_before_stopping_int]
		persist: false,
		scaleimage: 'both', //valid values are 'both', 'width', or 'none'
		fadeduration: 500, //transition duration (milliseconds)
		oninit:function(){ //event that fires when gallery has initialized/ ready to run
		},
		onslide:function(curslide, i){ //event that fires after each slide is shown
			//curslide: returns DOM reference to current slide's DIV (ie: try alert(curslide.innerHTML)
			//i: integer reflecting current image within collection being shown (0=1st image, 1=2nd etc)
		}
	})
	
	</script>

*Step 3:* Then, add the below sample markup to your page:

	<div id="simplegallery1" class="simplegallery"></div>

## Simple Controls Gallery set up ##

See script project page for additional details on setup and documentation: <http://www.dynamicdrive.com/dynamicindex4/simplegallery.htm>
