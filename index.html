<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
    <title>Midcolors</title>

    <style> 
		
		html, body {
			margin: 0;
			padding: 0;
			text-align: center;
			font-family: Arial, sans-serif;
		}

		.lcolorDiv, .rcolorDiv, .nbDiv {
			display: inline-block;
			vertical-align: top;
			margin: 40px;
		}

		.generateDiv, .errors {
			display: block;
			margin: 20px;
		}

		input, button {
			display: block;
			margin: 10px;
			text-align: center;
		}

		span {
			display: block;
		}

		.color1, .color2, .colors {
			width: 100px;
			height: 100px;
			cursor: pointer;
		}
		
		.colorDiv > *, 
		.midcolors > * {
			display: inline-block;
		}

		.alert {
			margin: auto;
			width: 400px;
		}

	</style>

    <!-- Bootstrap -->
    <link href="bootstrap/css/bootstrap.min.css" rel="stylesheet">

    <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
    <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
    <!--[if lt IE 9]>
      <script src="https://oss.maxcdn.com/html5shiv/3.7.3/html5shiv.min.js"></script>
      <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
    <![endif]-->
  </head>
  <body>

  <h1>Midcolors</h1>

  	<div class="jumbotron">
			<p>
			RGB color like this : rgb(0, 0, 0)<br>
			Hex color like this : #ffffff or #fff<br>
			HTML color name like this : blue</p>
   	</div>
   
   	<div class="lcolorDiv form-group">
		<p>First color :</p>
		<input type="text" class="lcolor form-control" placeholder='RGB, Hex or Name'>
	</div>
	<div class="nbDiv form-group">
		<p>Number of intermediate colors :</p>
		<input type="text" class="nb form-control" placeholder='Max : 10'><br>
	</div>
	<div class="rcolorDiv form-group">
		<p>Second color :</p>
		<input type="text" class="rcolor form-control" placeholder='RGB, Hex or Name'>
	</div>


	<div class="generateDiv">
		<button class="generate btn btn-default">Generate</button>
	</div>


	<div class="colorDiv">
		<div class="color color1"></div>

		<div class="midcolors"></div>

		<div class="color color2"></div>
	</div>

	<div class="errors"></div>


    <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
    <!-- Include all compiled plugins (below), or include individual files as needed -->
    <script src="bootstrap/js/bootstrap.min.js"></script>


	<script>
	
	function getRGB(str){
	  var match = str.match(/rgba?\((\d{1,3}), ?(\d{1,3}), ?(\d{1,3})\)?(?:, ?(\d(?:\.\d?))\))?/);
	  return match ? {
	    red: match[1],
	    green: match[2],
	    blue: match[3]
	  } : {};
	}

	$(document).ready(function() {

		/*	Generate */
		$('.generate').click(function() {
			// Reset midcolors
			$('.midcolors').html("");
			$('.errors').html("");

			var nb = parseInt($('.nb').val());
			var color1 = $('.lcolor').val();
			var color2 = $('.rcolor').val();

			if (nb > 10 || nb < 1 || !$.isNumeric(nb)) {
				$('.nb').css('color', 'red');
				$("<div class=\"alert alert-dismissible alert-danger\">  <button type=\"button\" class=\"close\" data-dismiss=\"alert\">&times;</button> <strong>Warning!</strong> Number must be less or equal to 10</div>").appendTo('.errors');
			} else {
				$('.nb').css('color', 'gray');
				$("<div class=\"alert alert-dismissible alert-success\">  <button type=\"button\" class=\"close\" data-dismiss=\"alert\">&times;</button> <strong>OK!</strong> Now click a color to copy it to the clipboard</div>").appendTo('.errors');

				$('.color1').css('background', color1);
				$('.color2').css('background', color2);
	
				var color1 = getRGB($('.color1').css('backgroundColor'));
				var color2 = getRGB($('.color2').css('backgroundColor'));
	
				var midRed = [];
				var midGreen = [];
				var midBlue = [];
	
				var tempRed = Math.floor(Math.abs(color1['red'] - color2['red'])/(nb+1));
				var tempGreen = Math.floor(Math.abs(color1['green'] - color2['green'])/(nb+1));
				var tempBlue = Math.floor(Math.abs(color1['blue'] - color2['blue'])/(nb+1));
	
				for (var i = 0 ; i < nb ; i++) {
					if (parseInt(color1['red']) < parseInt(color2['red'])) {
						midRed[i] = parseInt(color1['red']) + ((tempRed) * (i+1));
					}
					else {
						midRed[i] = parseInt(color1['red']) - ((tempRed) * (i+1));
					}

					if (parseInt(color1['green']) <= parseInt(color2['green']))
						midGreen[i] = parseInt(color1['green']) + ((tempGreen) * (i+1));
					else
						midGreen[i] = parseInt(color1['green']) - ((tempGreen) * (i+1));

					if (parseInt(color1['blue']) <= parseInt(color2['blue']))
						midBlue[i] = parseInt(color1['blue']) + ((tempBlue) * (i+1));
					else
						midBlue[i] = parseInt(color1['blue']) - ((tempBlue) * (i+1));

					$('<div class="colors" id="colors'+i+'" style="background:rgb('+midRed[i]+', '+midGreen[i]+', '+midBlue[i]+');"></div>').appendTo('.midcolors');

					$('.colors').click(function() {

						$('.errors').html("");

						var $temp = $('<input>');
						$('body').append($temp);
						$temp.val($(this).css('backgroundColor')).select();
						document.execCommand('copy');
						$temp.remove();

						$("<div class=\"alert alert-dismissible alert-success\">  <button type=\"button\" class=\"close\" data-dismiss=\"alert\">&times;</button> Color copied to clipboard!</div>").appendTo('.errors');
			
					});
					
				}
			}

		});

	});
		

	</script>

  </body>
</html>
