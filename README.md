#cleditor-imageupload-plugin

This is simple plug-in for [CLEditor](http://premiumsoftware.net/cleditor) simple, lightweight jQuery plugin (WYSIWYG editor). 

This plugin allows to download and use the downloaded pictures.

##Usage:

Add to your .html file next several lines.

to "&lt;head&gt;" path:
```html
	<link rel="stylesheet" media="screen" href="css/bootstrap.css"/>	
	<link rel="stylesheet" href="js/cleditor/jquery.cleditor.css" type="text/css">

	<script type="text/javascript" src="js/jquery-{version}.js"></script>	
	<script type="text/javascript" src="js/cleditor/jquery.cleditor.js"></script>
	<script type="text/javascript" src="js/cleditor-imageupload-plugin.js"></script>
	<script type="text/javascript">
		$(document).ready(function() {
			// Url for file upload 
			$.cleditor.buttons.image.uploadUrl = 'image-upload.html';
			// Url for images list
			$.cleditor.buttons.image.imageListUrl = 'image-list.json';
	
			$.cleditor.defaultOptions.width = 600;
			$.cleditor.defaultOptions.height = 300;
			$("#input").cleditor();
     });
   </script>
```


to "&lt;body&gt;" path:	
```html
	<textarea id="input" name="input"></textarea>	
	<script src="js/bootstrap.min.js"></script>	
```	
	
