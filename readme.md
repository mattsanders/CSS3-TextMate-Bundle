# CSS3 Textmate Bundle

By Matthew Sanders—matt@optionshft.com

<img src="https://a248.e.akamai.net/assets.github.com/img/d8be2ae65102914853b84f952086c42237055174/687474703a2f2f6d6174746865776e736172612e636f6d2f696d616765732f70726f73706574746976612d7468656d652d707265766965772e706e67" alt="CSS3 TextMate Bundle - Preview" />

Includes snippets for vendor-specific properties and (later) syntax highlighting.

## Installation

The best way to install this bundle is via command line. Simply copy & paste each line into a terminal window.

### Install via Git:

		mkdir -p ~/Library/Application\ Support/TextMate/Bundles
		cd ~/Library/Application\ Support/TextMate/Bundles
		git clone git@github.com:mattsanders/CSS3-TextMate-Bundle.git "CSS3.tmbundle"
		osascript -e 'tell app "TextMate" to reload bundles'

Source can be viewed or forked via GitHub: [http://github.com/mattsanders/CSS3-TextMate-Bundle/tree/master](http://github.com/mattsanders/CSS3-TextMate-Bundle/tree/master)

### Install without Git:

		mkdir -p ~/Library/Application\ Support/TextMate/Bundles
		cd ~/Library/Application\ Support/TextMate/Bundles
		wget http://github.com/mattsanders/CSS3-TextMate-Bundle/tarball/master
		tar zxf mattsanders-CSS3-TextMate-Bundle*.tar.gz
		rm mattsanders-CSS3-TextMate-Bundle*.tar.gz
		mv mattsanders-CSS3-TextMate-Bundle* CSS3.tmbundle
		osascript -e 'tell app "TextMate" to reload bundles'

## Basic Commands

These are the basic commands you may use for [TAB]-completion with your stylesheets.

* animation ( CSS Animations )
* radius ( border-radius in every combination )
* boxshadow
* gradient ( Cross Browser CSS Gradients )
* nth
* columns 
* textstroke 
* taphighlight ( Mobile Webkit )
* textshadow 
* transition ( CSS Transitions )
* userfocus 
* usermodify 
* userselect 
* rgba 
* hsla
* hsl

### CSS Template

Select File > New From Template > CSS3 > CSS Template

## Example

	-webkit-user-select:none; /* Webkit */
	   -moz-user-select:none; /* Mozilla */
	     -o-user-select:none; /* Opera */
	        user-select:none; /* Universal */

## Author

Matthew Sanders, matt@optionshft.com

Website [http://optionshft.com](http://optionshft.com) 
Twitter [http://twitter.com/mattsanders](http://twitter.com/mattsanders)
Dribbble [http://dribbble.com/matthew](http://dribbble.com/matthew)



License
=======

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/80x15.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">CSS3 TextMate Bundle</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://optionshft.com" property="cc:attributionName" rel="cc:attributionURL">Matthew Sanders</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative Commons Attribution-ShareAlike 3.0 Unported License</a>.