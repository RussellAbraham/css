# CSS



animation
animation-delay
animation-direction
animation-duration
animation-fill-mode
animation-iteration-count
animation-name
animation-play-state
animation-timing-function


break-after
break-before
break-inside

display

filter

float


font
@font-face
font-family
font-feature-settings
font-kerning
font-size
font-size-adjust
font-stretch
font-style
font-variant
font-variant-caps
font-weight



list-style
list-style-image
list-style-position
list-style-type


mix-blend-mode

opacity

order


page-break-after
page-break-before
page-break-inside

perspective
perspective-origin


resize


transform
transform-origin
transform-style

transition
transition-delay
transition-duration
transition-property
transition-timing-function


unicode-bidi

visibility



z-index






.hide, 
.hide:after { opacity : 0; }
.hide:before { opacity : 1;	 }

.show:before {	 opacity : 0; }
.show:after { opacity : 1; }

will-change : ;

opacity : ;

transition : ;
- skew is the one that doesnt repaint any layers, opacity too

transition-property : ;

transition-duration: 0s, 0s, 0s, 0s;

transition-delay: 0s, 0s, 0s, 0s;

transition-timing-function : ;  


transform:;

animation : ;
animation-delay: -1s;
animation-duration: 1s;

@media (any) {}

Media Types

@media screen {
  body {}
}

@media print {
  body {}
}

@media all {}

@media only screen and (orientation: landscape) {
  body {}
}

@media only screen and (orientation: portrait) {
  body {}
}

@media (prefers-reduced-motion: reduce) {
  .accelerator {
    transition : none;
  }
}

.row::after {
  content: "";
  clear: both;
  display: block;
}

[class*="col-"] {
  float: left;
  padding: 15px;
}
/* For desktop: */
.col-1 {width: 8.33%;}
.col-2 {width: 16.66%;}
.col-3 {width: 25%;}
.col-4 {width: 33.33%;}
.col-5 {width: 41.66%;}
.col-6 {width: 50%;}
.col-7 {width: 58.33%;}
.col-8 {width: 66.66%;}
.col-9 {width: 75%;}
.col-10 {width: 83.33%;}
.col-11 {width: 91.66%;}
.col-12 {width: 100%;}

@media only screen and (max-width: 768px) {
  /* For mobile phones: */
  [class*="col-"] {
    width: 100%;
  }
}

Examples of dynamic css

<link rel="stylesheet" media="mediatype and|not|only (expressions)" href="print.css">

@media screen and (max-width: 900px) and (min-width: 600px), (min-width: 1100px) {

}

@media screen and (min-width: 320px) {
  html {
    font-size: calc(16px + 4 * ((100vw - 320px) / 880));
  }
}
@media screen and (min-width: 320px) {
  body {
    font-size: calc(35.152px + 30.384 * ((100vw - 320px) / 880));
  }
}

@keyframes {
	from {}
	to {}
}

@keyframes {
  	0%, 100% {}
	  50%{}
}


.accelerator:before {}

.accelerator:before,
.accelerator:after {}
  
.accelerator:after {}
