# CSS Level 3—Textmate Bundle

By Matthew Sanders—matt@optionshft.com


Installation
============

To install via Git:

		mkdir -p ~/Library/Application\ Support/TextMate/Bundles
		cd ~/Library/Application\ Support/TextMate/Bundles
		git clone git@github.com:mattsanders/CSS3-TextMate-Bundle.git "CSS3.tmbundle"
		osascript -e 'tell app "TextMate" to reload bundles'

Source can be viewed or forked via GitHub: [http://github.com/mattsanders/CSS3-TextMate-Bundle/tree/master](http://github.com/mattsanders/CSS3-TextMate-Bundle/tree/master)

To install without Git:

		mkdir -p ~/Library/Application\ Support/TextMate/Bundles
		cd ~/Library/Application\ Support/TextMate/Bundles
		wget http://github.com/mattsanders/CSS3-TextMate-Bundle/tarball/master
		tar zxf mattsanders-CSS3-TextMate-Bundle*.tar.gz
		rm mattsanders-CSS3-TextMate-Bundle*.tar.gz
		mv mattsanders-CSS3-TextMate-Bundle* CSS3.tmbundle
		osascript -e 'tell app "TextMate" to reload bundles'

## Basic Commands

* radius [ tab completion ]
* boxshadow [ tab completion ]
* gradient [ tab completion ]
* nth [ tab completion ]
* columns [ tab completion ]
* textstroke [ tab completion ]
* taphighlight [ tab completion ]
* textshadow [ tab completion ]
* transition [ tab completion ]
* userfocus [ tab completion ]
* usermodify [ tab completion ]
* userselect [ tab completion ]
* rgba [ tab completion ]


## Output
=========

/* style.css */

/* Author: Matthew Sanders */

/* Reset */

	* { outline:0 !important; -webkit-font-smoothing:antialiased; text-rendering:optimizeLegibility; }

/* Language specification for smart quotes */
	:lang(en-us) >q { quotes:"\201c" "\201d" "\2018" "\2019"; }
	:lang(en-gb) >q { quotes:"\2018" "\2019" "\201c" "\201d"; }

	body { margin:0; padding:0; }


/* Structure */
property { 
-webkit-border-radius:5px; /* Saf3+, Chrome */
   -moz-border-radius:5px; /* FF1+ */
        border-radius:5px; /* Opera 10.5, IE 9 */ 	


 -webkit-border-top-left-radius:5px; /* Saf3+, Chrome */
-webkit-border-top-right-radius:5px;
	  -moz-border-radius-topleft:5px; /* FF1+ */
	 -moz-border-radius-topright:5px;
	      border-top-left-radius:5px; /* Opera 10.5, IE 9 */ 
	     border-top-right-radius:5px; 	


-webkit-border-bottom-right-radius:5px; /* Saf3+, Chrome */
 -webkit-border-bottom-left-radius:5px;
    -moz-border-radius-bottomright:5px; /* FF1+ */
     -moz-border-radius-bottomleft:5px;
        border-bottom-right-radius:5px; /* Opera 10.5, IE 9 */
         border-bottom-left-radius:5px;  


-webkit-box-shadow:0px 0px 4px rgba(0,0,0,0.2); /* Saf3.0+, Chrome */
   -moz-box-shadow:0px 0px 4px rgba(0 0 0 0.2); /* FF3.5+ */
        box-shadow:0px 0px 4px rgba(0 0 0 0.2); /* Opera 10.5, IE 9.0 */
    filter:progid:DXImageTransform.Microsoft.dropshadow(OffX=0px, OffY=0px, Color='#fff'); /* IE6,IE7 */
-ms-filter:"progid:DXImageTransform.Microsoft.dropshadow(OffX=0px, OffY=0px, Color='#fff')"; /* IE8 */ 


-webkit-box-shadow:0px 0px 4px #ffffff; /* Saf3.0+, Chrome */
   -moz-box-shadow:0px 0px 4px #ffffff; /* FF3.5+ */
        box-shadow:0px 0px 4px #ffffff; /* Opera 10.5, IE 9.0 */
    filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=0px, OffY=0px, Color='#ffffff'); /* IE6,IE7 */
-ms-filter:"progid:DXImageTransform.Microsoft.dropshadow(OffX=0px, OffY=0px, Color='#ffffff')"; /* IE8 */ 


background:#fff; /* Old browsers */
background:-moz-linear-gradient(top, #fff 0%, #e5e5e5 100%); /* FF3.6+ */
background:-webkit-gradient(linear, left top, left bottom, color-stop(0%,#fff), color-stop(100%,#e5e5e5)); /* Chrome,Safari4+ */
background:-webkit-linear-gradient(top, #fff 0%,#e5e5e5 100%); /* Chrome10+,Safari5.1+ */
background:-o-linear-gradient(top, #fff 0%,#e5e5e5 100%); /* Opera11.10+ */
background:-ms-linear-gradient(top, #fff 0%,#e5e5e5 100%); /* IE10+ */
filter:progid:DXImageTransform.Microsoft.gradient( startColorstr='#fff', endColorstr='#e5e5e5',GradientType=0 ); /* IE6-9 */
background:linear-gradient(top, #fff 0%,#e5e5e5 100%); /* W3C */ 


background:#fff; /* Old browsers */
background:-moz-linear-gradient(left, #fff 10%, #e5e5e5 100%); /* FF3.6+ */
background:-webkit-gradient(linear, left top, right top, color-stop(10%,#fff), color-stop(100%,#e5e5e5)); /* Chrome,Safari4+ */
background:-webkit-linear-gradient(left, #fff 10%,#e5e5e5 100%); /* Chrome10+,Safari5.1+ */
background:-o-linear-gradient(left, #fff 10%,#e5e5e5 100%); /* Opera11.10+ */
background:-ms-linear-gradient(left, #fff 10%,#e5e5e5 100%); /* IE10+ */
filter:progid:DXImageTransform.Microsoft.gradient( startColorstr='#fff', endColorstr='#e5e5e5',GradientType=1 ); /* IE6-9 */
background:linear-gradient(left, #fff 10%,#e5e5e5 100%); /* W3C */ 


:nth-child(even)
:nth-child(odd)


-webkit-column-count:2; 
-webkit-column-rule:1px solid #bbb;
-webkit-column-gap:2em; 


-webkit-text-fill-color:black;
-webkit-text-stroke-color:red;
-webkit-text-stroke-width:1.50px; 


-webkit-tap-highlight-color:rgba(0,0,0,0.1); 


text-shadow:rgba(64, 64, 64, 0.5) 2px 2px 2px; 


-webkit-transition:color(property) .25s(duration) linear(timing-function) .1s(delay);		
   -moz-transition:color(property) .25s(duration) linear(timing-function) .1s(delay);
        transition:color(property) .25s(duration) linear(timing-function) .1s(delay); 


-webkit-transition-property:opacity | none | all | [ <IDENT> ] [ ‘,’ <IDENT> ]*;
   -moz-transition-property:opacity | none | all | [ <IDENT> ] [ ‘,’ <IDENT> ]*; 
        transition-property:opacity | none | all | [ <IDENT> ] [ ‘,’ <IDENT> ]*; 


-webkit-transition-duration:0.1s;		
   -moz-transition-duration:0.1s;
        transition-duration:0.1s; 


-webkit-transition-timing-function:ease | linear | ease-in | ease-out | ease-in-out | cubic-bezier(<number>, <number>, <number>, <number>) [, ease | linear | ease-in | ease-out | ease-in-out | cubic-bezier(<number>, <number>, <number>, <number>)]*;		
   -moz-transition-timing-function:ease | linear | ease-in | ease-out | ease-in-out | cubic-bezier(<number>, <number>, <number>, <number>) [, ease | linear | ease-in | ease-out | ease-in-out | cubic-bezier(<number>, <number>, <number>, <number>)]*;
        transition-timing-function:ease | linear | ease-in | ease-out | ease-in-out | cubic-bezier(<number>, <number>, <number>, <number>) [, ease | linear | ease-in | ease-out | ease-in-out | cubic-bezier(<number>, <number>, <number>, <number>)]*; 


-webkit-transition-delay:0.5s;		
   -moz-transition-delay:0.5s;
        transition-delay:0.5s; 


-webkit-user-focus:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Webkit */
   -moz-user-focus:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Mozilla */
     -o-user-focus:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Opera */
        user-focus:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Universal */ 


-webkit-user-focus-key:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Webkit */
   -moz-user-focus-key:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Mozilla */
     -o-user-focus-key:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Opera */
        user-focus-key:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Universal */ 


-webkit-user-focus-pointer:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Webkit */
   -moz-user-focus-pointer:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Mozilla */
     -o-user-focus-pointer:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Opera */
        user-focus-pointer:auto | normal | select-all | select-before | select-after | select-same | select-menu | inherit; /* Universal */ 


-webkit-user-modify:read-only | read-write | write-only | inherit; /* Webkit */
   -moz-user-modify:read-only | read-write | write-only | inherit; /* Mozilla */
     -o-user-modify:read-only | read-write | write-only | inherit; /* Opera */
        user-modify:read-only | read-write | write-only | inherit; /* Universal */ 


-webkit-user-select:none | text | toggle | element | elements | all | inherit; /* Webkit */
   -moz-user-select:none | text | toggle | element | elements | all | inherit; /* Mozilla */
     -o-user-select:none | text | toggle | element | elements | all | inherit; /* Opera */
        user-select:none | text | toggle | element | elements | all | inherit; /* Universal */ 


rgba(255, 0, 0, 0.75); }


## Author

Matthew Sanders, matt@optionshft.com, [http://optionshft.com](http://optionshft.com) Twitter [http://twitter.com/mattsanders](http://twitter.com/mattsanders)



License
=======


(The MIT License)

Copyright (c) 2011 Matthew Sanders, matt@optionshft.com

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.