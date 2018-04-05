---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
---
<header>
    <nav class="navigation bg">
    	<div class="container">
			<a class="logo" href="/">
				<img src="images/Leanplum_Logo_White.png" alt="Leanplum" height="20">
			</a>
	    </div>
    </nav>
    <script type="text/javascript" src="leanplum.js"></script>
	<script type="text/javascript">
		// This value should be set to true only if you're developing on your server.
		var isDevelopmentMode = true;
		 
		// Sample variables. This can be any JSON object.
		var variables = {
		  items: {
		    color: 'red',
		    size: 20,
		    showBadges: true
		  },
		  showAds: true
		};
		 
		// We've inserted your Craig's DailyTracker API keys here for you :)
		if (isDevelopmentMode) {
		  Leanplum.setAppIdForDevelopmentMode("app_ELqc6tF6WusSEk4oRiudRhqoU5O6CsUaWLvNid8x3as", "dev_vYJLCLGD77s9GtMiF0gHdRoMiZsrryPa7vMBkPKCZXg");
		} else {
		  Leanplum.setAppIdForProductionMode("app_ELqc6tF6WusSEk4oRiudRhqoU5O6CsUaWLvNid8x3as", "prod_4MnVJvhw8hQyHSFVScebg9NDRdkUkwRuI9XQDWAQsB4");
		}
		 
		Leanplum.setVariables(variables);
		Leanplum.start(function(success) {
		  console.log('Success: ' + success);
		  console.log('Variables', Leanplum.getVariables());
		});
		Leanplum.track('HTML5 SDK triggered')
	</script>
</header>
<div class="container-fluid">
	<div class="row">
		<div class="col-md-3">
			 <button class="btn btn-primary">Trigger event 1</button>
			 <script type="text/javascript">
			 	Leanplum.track("web trigger 1");
			 	console.log('web trigger 1');

			 </script>
		</div>
		<div class="col-md-3">
			 <button class="btn btn-primary">Trigger event 2</button>
		</div>
		<div class="col-md-3">
			 <button class="btn btn-primary">Trigger event 3</button>
		</div>
		<div class="col-md-3">
			 <button class="btn btn-primary">Trigger event 4</button>
		</div>
	</div>
</div>
<br>
<div class="container-fluid">
	<div class="row">
		<div class="col-md-4">
			<img src="images/a_bg1.png">
		</div>
		<div class="col-md-4">
			<img src="images/a_bg2.png">
		</div>
		<div class="col-md-4">
			<img src="images/a_bg3.png">
		</div>
	</div>
	<div class="row">
		<div class="col-md-4">
			<img src="images/a_bg6.png">
		</div>
		<div class="col-md-4">
			<img src="images/a_bg7.png">
		</div>
		<div class="col-md-4">
			<img src="images/a_bg8.png">
		</div>
	</div>
	<div class="row">
		<div class="col-md-4">
			<img src="images/a_bg9.png">
		</div>
		<div class="col-md-4">
			<img src="images/a_bg1.png">
		</div>
		<div class="col-md-4">
			<img src="images/a_bg2.png">
		</div>
	</div>
</div>
<script
  src="https://code.jquery.com/jquery-3.2.1.min.js"
  integrity="sha256-hwg4gsxgFZhOsEEamdOYGBf13FyQuiTwlAQgxVSNgt4="
  crossorigin="anonymous"></script>
<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

<!-- Optional theme -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">

<!-- Latest compiled and minified JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
