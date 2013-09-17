#Bootjack Datepicker

Bootjack datepicker component is a datepicker component of [Bootjack](http://github.com/rikulo/bootjack).

* [Home](http://rikulo.org)
* [Git Repository](https://github.com/rikulo/bootjack-datepicker)
* [Discussion](http://stackoverflow.com/questions/tagged/rikulo)
* [Issues](https://github.com/rikulo/bootjack-datepicker/issues)

##Install from Dart Pub Repository

Include the following in your `pubspec.yaml`:

    dependencies:
      bootjack_datepicker: any

Then run the [Pub Package Manager](http://pub.dartlang.org/doc) in Dart Editor (Tool > Pub Install). If you are using a different editor, run the command
(comes with the Dart SDK):

    pub install

##Usage

First of all in your HTML file, you need to include the CSS resource:
  
	<head>
		...
		<link rel="stylesheet" href="packages/bootjack_datepicker/css/bootjack-datepicker.min.css">
	</head>

###Embedded calendar
To create a calendar component to your HTML page, add `class="calendar"` to the element you want to attach to (most typically this would be the `<div>`).
	
	<div class="calendar" data-date="2013/09/16" data-format="yyyy/MM/dd"></div>
	
Then call the following global registration in Dart:

	void main() {
		Calendar.use();
	}
	
###Datepicker
Using a calendar component in a dropdown div element as a date picker component, add `class="calendar"` to the element you want to attach to, 
then add the `data-target` attribute with the ID or class of the element that you want to display the date value.
	
	<div class="input-group">
		
	  <input id="inp" type="text" class="form-control">
	  
	  <span class="input-group-btn">
		
		<button id="btn" class="btn btn-default dropdown-toggle" type="button" 
		  data-toggle="dropdown" data-target="#">
		  <span class="glyphicon glyphicon-calendar"></span>
		</button>
		
		<div class="dropdown-menu" >
			<div class="calendar" data-date="2013/09/16" data-format="yyyy/MM/dd"
				data-target="#inp"></div>
		</div>
		
	  </span>
	</div>
	
Then call the following global registration in Dart:

	void main() {
		Calendar.use();
	}
	
Check more [examples](https://github.com/rikulo/bootjack-datepicker/tree/master/example).
	
##Notes to Contributors

###Test and Debug

You are welcome to submit [bugs and feature requests](https://github.com/rikulo/bootjack-datepicker/issues). Or even better if you can fix or implement them!

###Fork Bootjack Datepicker

If you'd like to contribute back to the core, you can [fork this repository](https://help.github.com/articles/fork-a-repo) and send us a pull request, when it is ready.

Please be aware that one of Rikulo's design goals is to keep the sphere of API as neat and consistency as possible. Strong enhancement always demands greater consensus.

If you are new to Git or GitHub, please read [this guide](https://help.github.com/) first.
