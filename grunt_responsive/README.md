# Grunt Responsive Template
## Features
- 3 Layout responsive ( desktop , tablet , mobile )
- Best view IE9+
- SCSS, compass
- SVG Icon : SVG or PNG Fallback ( GRUNTICON )
- Minified JS : Concat JS files into one JS File (and minified Optional)
- BrowserSync : Testing workflow faster by synchronising URLs, interactions and code changes across multiple devices
- Grunt environment choose: default / prod

## Step to use
Step 1: Clone this template set to your project folder

Step 2: Download Node.js in [https://nodejs.org/en/](https://nodejs.org/en/)

Step 3: Install npm -- [Tutorial](https://docs.npmjs.com/getting-started/installing-node)
```
npm install npm -g
```
Step 4: Install grunt -- [Tutorial](http://gruntjs.com/getting-started)
```
npm install -g grunt-cli
```
Step 5. Install bower -- [Tutorial](https://bower.io/#install-bower)
```
npm install -g bower
```
Step 6. Go to your project folder path
```
cd C:\project\client\project-name
```
Step 7. Run below command in every new project. It will generate assigned plugin component to "node_modules" and "bower_components" folder.
**_BUT DO NOT COMMIT ON SVN DUE TO THE LARGE AMOUNT OF FOLDERS_**
```
npm install
bower install
```
Step 8. Run grunt to watch folder. It will success with open new window with localhost testing server
```
grunt
```
Step 9. Browser will auto refresh with any changes

Step 10. Or you may output as production mode which minified all js/css files.
```
grunt prod
```

## Bower plugin List
- jquery: ~1.10.2
- jquery.easing: ~1.3.1
- jquery-mousewheel : ~3.1.13
- modernizr: ~2.6.2
- magnific-popup : ~1.1.0
- jScrollPane : ~2.0.23
- jquery-selectric : ~1.9.6
- jquery.inview : 1.1.2
- smoothscroll-for-websites : ~1.4.4

## Grunt plugin List
- grunt: ~0.4.4
- grunt-bower-concat: ~1.0.0
- grunt-contrib-concat: ~1.0.1
- grunt-contrib-jshint: ~1.0.0
- jshint-stylish: ~2.2.0
- grunt-contrib-uglify: ~1.0.1
- grunt-contrib-watch: ~1.0.0
- grunt-contrib-imagemin : ~1.0.1
- grunt-contrib-compass : ~1.1.1
- grunt-grunticon : ~2.2.1
- grunt-browser-sync : ~2.2.0

## Common Commard
### Popup Magnific popup box
```
popupBox( $(TARGET), {
	showCloseBtn : true,
	fixedContentPos : true,
	fixedBgPos : true,
	closeOnBgClick: true,
	callbacks:{
		open: function(){

		},
		close: function(){
		
		}
	}
});
```
### Popup Alert Msg
```
alertMsg( 'MSG HERE', config);
```
### Popup Youtube Video
```
videoPop( youtubeID , config );
```
### Inview effect
```
> It will add a class "play" when inview
<div class="invew"></div>
```
### Scroll to target function
```
scrollto('.TARGET');
```
### ImgSlider Usage
```
newSliderName = new imgSlider( $('target'), {
	speed: 300,
	drag: true,
	loop: true,
	autoHeight: false,
	autoPlay: false,
	autoPlaySpeed: 5000,
	fade: false,
	offsetWidth: 1,
	thumbnailCarousel: true,
	beforeSlideCallback: function(){
	},
	afterSlideCallback: function(){
	}
});

gBannerSlider.transition( 'next' , idx );
gBannerSlider.transition( 'prev' , idx );
gBannerSlider.changePattern( idx );
gBannerSlider.slidesOnReady();
gBannerSlider.destroy();
```
