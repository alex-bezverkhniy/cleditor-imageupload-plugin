This is simple plug-in for CLEditor. Allows to download and use the downloaded pictures. 

Usage:

Add to your .html file next several lines.

to "head" path:
<head>
	...
	<!-- "bootstrap" styles -->
	<link rel="stylesheet" media="screen" href="css/bootstrap.css"/>
	<!-- "cleditor" styles -->
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
	...
</head>

to "body" path:

<body>
	...
	<!-- Target field -->
	<textarea id="input" name="input"></textarea>
	<!-- Script for "bootstrap" functionality -->
	<script src="js/bootstrap.min.js"></script>	
	...
</body>