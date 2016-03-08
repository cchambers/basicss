Introduction
=======================
Basicss is an object-oriented scaling CSS framework. The real beauty of OO CSS is that the classes explain themselves. I will break down each group of rules that are included in the following sections...

### Major Change Log: 
- v3 - Padding removed entirely from content flow system to encourage nesting.  
- v3.4.5 - Added portrait orientation to "touch" breakpoint.  
- v4 - "desktop" and "touch" deprecated - replaced with "high-on/high-off" and "low-on/low-off".  

OOCSS
-----
### Box Modifications
#### Model
    .no-pad             { padding: 0 !important }
    .pad,   
    .pad-box            { padding: 30px; padding: 3rem }
    .pad-sides          { padding-left: 30px; padding-right: 30px; padding-left: 3rem; padding-right: 3rem }
    .pad-lips           { padding-top: 30px; padding-bottom: 30px; padding-top: 3rem; padding-bottom: 3rem }
    .pad-top            { padding-top: 30px; padding-top: 3rem }
    .pad-bottom         { padding-bottom: 30px; padding-bottom: 3rem }
    .pad-right          { padding-right: 30px; padding-right: 3rem }
    .pad-left           { padding-left: 30px; padding-left: 3rem; }
    .pad-light,
    .pad-box-light      { padding: 15px; padding: 1.5rem; }
    .pad-sides-light    { padding-left: 15px; padding-right: 15px; padding-left: 1.5rem; padding-right: 1.5rem }
    .pad-lips-light     { padding-top: 15px; padding-bottom: 15px; padding-top: 1.5rem; padding-bottom: 1.5rem }
    .pad-top-light      { padding-top: 15px; padding-top: 1.5rem }
    .pad-bottom-light   { padding-bottom: 15px; padding-bottom: 1.5rem }
    .pad-right-light    { padding-right: 15px; padding-right: 1.5rem }
    .pad-left-light     { padding-left: 15px; padding-left: 1.5rem }
    .pad-hard,
    .pad-box-hard       { padding: 60px; padding: 6rem }
    .pad-sides-hard     { padding-left: 60px; padding-right: 60px; padding-left: 6rem; padding-right: 6rem }
    .pad-lips-hard      { padding-top: 60px; padding-bottom: 60px; padding-top: 6rem; padding-bottom: 6rem }
    .pad-top-hard       { padding-top: 60px; padding-top: 6rem }
    .pad-bottom-hard    { padding-bottom: 60px; padding-bottom: 6rem }
    .pad-right-hard     { padding-right: 60px; padding-right: 6rem }
    .pad-left-hard      { padding-left: 60px; padding-left: 6rem }

    .margin,    
    .margin-box         { margin: 30px; margin: 3rem }
    .margin-top         { margin-top: 30px; margin-top: 3rem }
    .margin-bottom      { margin-bottom: 30px; margin-bottom: 3rem; }
    .margin-right       { margin-right: 30px; margin-right: 3rem }
    .margin-left        { margin-left: 30px; margin-left: 3rem }
    .margin-sides       { margin-left: 30px; margin-right: 30px; margin-left: 3rem; margin-right: 3rem }
    .margin-lips        { margin-top: 30px; margin-bottom: 30px; margin-top: 3rem; margin-bottom: 3rem }
    .margin-light,
    .margin-box-light   { margin: 15px; margin: 1.5rem }
    .margin-top-light   { margin-top: 15px; margin-top: 1.5rem }
    .margin-bottom-light{ margin-bottom: 15px; margin-bottom: 1.5rem }
    .margin-right-light { margin-right: 15px; margin-right: 1.5rem }
    .margin-left-light  { margin-left: 15px; margin-left: 1.5rem }
    .margin-sides-light { margin-left: 15px; margin-right: 15px; margin-left: 1.5rem; margin-right: 1.5rem }
    .margin-lips-light  { margin-top: 15px; margin-bottom: 15px; margin-top: 1.5rem; margin-bottom: 1.5rem }
    .margin-hard,       
    .margin-box-hard    { margin: 60px; margin: 6rem }
    .margin-top-hard    { margin-top: 60px; margin-top: 6rem }
    .margin-bottom-hard { margin-bottom: 60px; margin-bottom: 6rem }
    .margin-right-hard  { margin-right: 60px; margin-right: 6rem }
    .margin-left-hard   { margin-left: 60px; margin-left: 6rem }
    .margin-sides-hard  { margin-left: 60px; margin-right: 60px; margin-left: 6rem; margin-right: 6rem }
    .margin-lips-hard   { margin-top: 60px; margin-bottom: 60px; margin-top: 6rem; margin-bottom: 6rem }

    .pull-top           { margin-top: -30px; margin-top: -3rem }
    .pull-bottom        { margin-bottom: -30px; margin-bottom: -3rem }
    .pull-right         { margin-right: -30px; margin-right: -3rem }
    .pull-left          { margin-left: -30px; margin-left: -3rem }
    .pull-top-light     { margin-top: -15px; margin-top: -1.5rem }
    .pull-bottom-light  { margin-bottom: -15px; margin-bottom: -1.5rem }
    .pull-right-light   { margin-right: -15px; margin-right: -1.5rem }
    .pull-left-light    { margin-left: -15px; margin-left: -1.5rem }
    .pull-top-hard      { margin-top: -60px; margin-top: -6rem }
    .pull-bottom-hard   { margin-bottom: -60px; margin-bottom: -6rem }
    .pull-right-hard    { margin-right: -60px; margin-right: -6rem }
    .pull-left-hard     { margin-left: -60px; margin-left: -6rem }

#### HTML5 Columns
    .cols-2 { 
      -webkit-column-count: 2;
      -moz-column-count: 2;
      column-count: 2
    }
    .cols-3 { 
      -webkit-column-count: 3;
      -moz-column-count: 3;
      column-count: 3
    }

### Text Modifications  
#### Weights

    .ultralight{
      font-family: 'HelveticaNeue-UltraLight',
      'Helvetica Neue UltraLight',
      'Helvetica Neue', 
      Helvetica, Arial, Roboto, sans-serif;
      font-weight: 100 !important;
      letter-spacing: 1px
    }
    .light   { 
      font-family: "HelveticaNeue-Light", 
      "Helvetica Neue Light", 
      Helvetica, Arial, Roboto, sans-serif;
      font-weight: 300 !important;
    }
    .normal  {
      font-family: "Helvetica Neue", 
      Helvetica, Arial, Roboto, sans-serif;
      font-weight: normal !important;
    }
    .bold    {
      font-family: "Helvetica Neue", 
      Helvetica, Arial, Roboto, sans-serif;
      font-weight: 700 !important;
    }
    
#### Alignment
    .text-right     { text-align: right }
    .text-left      { text-align: left }
    .text-center    { text-align: center }
    .text-justify   { text-align: justify }
    .force-justify  { text-align: justify }
    .force-justify:after{
      display: inline-block;
      width: 100%;
      content: '.';
      height: 0;
      overflow: hidden;
}
    
#### Size
    .px100          { font-size: 100px; font-size: 10rem }
    .px98           { font-size: 98px; font-size: 9.8rem }
    ...
    .px12           { font-size: 12px; font-size: 1.2rem }
    .px10           { font-size: 10px; font-size: 1.0rem }
    
#### Case
    .normalcase     { text-transform: normal }
    .uppercase      { text-transform: uppercase }
    .lowercase      { text-transform: lowercase }
    .titlecase      { text-transform: capitalize }
    .strike         { text-decoration: line-through }
    .italic         { font-style: italic }

#### Line Height    
    .lh100          { line-height: 100px; line-height: 10rem }
    .lh98           { line-height: 98px; line-height: 9.8rem }
    ...
    .lh12           { line-height: 12px; line-height: 1.2rem }
    .lh10           { line-height: 10px; line-height: 1.0rem }


### Positioning  

    .center-box      { margin-left: auto; margin-right: auto }
    .float-none      { float: none !important }
    .float-left      { float: left !important }
    .float-right     { float: right !important }
    .absolute        { display: block; position: absolute }
    .relative        { display: block; position: relative }
    .fixed           { display: block; position: fixed }
    .static          { display: block; position: static }
    .clear           { clear: both; overflow: hidden }

In regards to absolute positioning, just add the `.absolute` class and proceed to add the edge distances in-line. This is where any javascript modification you make will be, and makes it easier for your content entry team to position elements freely. 

    <div class="absolute back-blue" style="top:100px;left:100px"> 
        I'm absolutely positioned!
    </div>
    
#### z-index
    .sub-layer       { position: relative; z-index: -1 }
    .back-layer      { position: relative; z-index: 1 }
    .middle-layer    { position: relative; z-index: 2 }
    .front-layer     { position: relative; z-index: 3 }
    
### Trigger Classes 

These classes are generally used to preload a class with properties that will be change eventually via a JavaScript Timer or some other event on the page.

    .fill            { position: absolute; width: 100%; height: 100% }
    .fill-height     { height: 100% }
    .fill-width      { width: 100% }
    .off             { display: none }
    .on,
    .block           { display: block }
    .on-inline,
    .inline          { display: inline-block }
    .alpha-off       { opacity: 0 }
    .alpha-on        { opacity: 1 }
    .stage-right     { left: 110% !important }
    .stage-left      { right: 110% !important }
    .stage-top       { bottom: 110% !important }
    .stage-bottom    { top: 110% !important }


### Scrollbar Control
    .overhide        { overflow: hidden }
    .overshow        { overflow: visible }
    .scroll-y        { overflow-y: scroll }

    
Flexbox 
-------
Flexbox is supported in most modern browsers, but implemented in too many ways to even try to remember. Here, I've tried to give some more semantic meaning to the confusing property soup that is flexbox.

### Flex Container
    .flex  {
       display: -webkit-box;
       display: -moz-box;
       display: -ms-flexbox;
       display: -ms-box;
       display: -webkit-flex;
       display: flex;
       flex-direction: row;
       -ms-flex-direction: row;
       flex-wrap: nowrap;
       -ms-flex-wrap: nowrap;
       justify-content: space-between;
       -ms-flex-pack: justify;
     }
     
The `.flex` class can be applied to any container to make the children capable of becoming flex-items. The default settings above make items justify themselves across a single row, but there are a number of class mods that can be applied...
     
#### Flex Container Modifications
    .flex.row        { flex-direction: row; -ms-flex-direction: row }
    .flex.row-rev    { flex-direction: row-reverse; -ms-flex-direction: row-reverse }
    .flex.col        { flex-direction: column; -ms-flex-direction: column }
    .flex.col-rev    { flex-direction: column-reverse; -ms-flex-direction: column-reverse }
    
Flex-items can be displayed as rows or columns, and even reversed. 

    .flex.wrap       { flex-wrap: wrap; -ms-flex-wrap: wrap }
    .flex.nowrap     { flex-wrap: nowrap; -ms-flex-wrap: nowrap }
    .flex.wrap-rev   { flex-wrap: wrap-reverse; -ms-flex-wrap: wrap-reverse }
    
The default setting is "nowrap", but if you want your elements to break to another line, you will need to change this by adding a `.wrap`.
    
    .flex.start      { justify-content: flex-start; -ms-flex-pack: start }
    .flex.end        { justify-content: flex-end; -ms-flex-pack: end }
    .flex.center     { justify-content: center; -ms-flex-pack: center }
    .flex.between    { justify-content: space-between; -ms-flex-pack: justify }
    .flex.around     { justify-content: space-around; -ms-flex-pack: justify }

    .flex.top        { align-content: flex-start; -ms-flex-align: start }
    .flex.bottom     { align-content: flex-end; -ms-flex-align: end }
    .flex.middle     { align-content: center; -ms-flex-align: center }
    .flex.stretch    { align-content: stretch; -ms-flex-align: stretch }
    .flex.content    { align-content: baseline; -ms-flex-align: baseline }

### Flex Item
    .flex-item {
      flex-grow: 0;
      flex-shrink:.5;
      flex-basis: auto
    }

    .flex-item.top    { align-self: flex-start; }
    .flex-item.bottom { align-self: flex-end; }
    .flex-item.middle { align-self: center; }
    .flex-item.stretch{ align-self: stretch; }
    .flex-item.content{ align-self: baselinet; }
     
#### Flex Item Modifications
    .flex-item.single  { flex-grow: 0 }
    .flex-item.double  { flex-grow: 1 }
    .flex-item.triple  { flex-grow: 2 }

Flex items are allowed to grow relative to their width. So, a `.single` with a width setting of 200px would grow no larger than 200px, while a `.double` flex-item could grow to 400px, etc.
    
    .order-0{ order: 0; -ms-box-ordinal: 0 }
    .order-1{ order: 1; -ms-box-ordinal: 1 }
    .order-2{ order: 2; -ms-box-ordinal: 2 }
    .order-3{ order: 3; -ms-box-ordinal: 3 }
    .order-4{ order: 4; -ms-box-ordinal: 4 }
    .order-5{ order: 5; -ms-box-ordinal: 5 }
    .order-6{ order: 6; -ms-box-ordinal: 6 }
    .order-7{ order: 7; -ms-box-ordinal: 7 }
    .order-8{ order: 8; -ms-box-ordinal: 8 }
    .order-9{ order: 9; -ms-box-ordinal: 9 }
    
Sometimes you may find the need to move a flex-item around in the stack... this is what the order property is used for! 

Content Flow Control
---------------
You can make any layout imaginable with this system. It doesn't work like a 'grid', per say... grids are generally padded. You can pad this system any way you want with the OO classes provided:

    .contain {
      width: 100rem;
      margin-left: auto;
      margin-right: auto
    }
    .row { width: 100%; float: left }
    [class`=col-] { float: left }

    .col-1-1 { width: 100% }
    .col-3-4 { width: 75% }
    .col-1-2 { width: 50% }
    .col-1-4 { width: 25% }
    .col-1-5 { width: 20% }
    .col-2-5 { width: 40% }
    .col-3-5 { width: 60% }
    .col-4-5 { width: 80% }
    .col-1-6 { width: calc( 100% / 6 ) }
    .col-5-6 { width: 83.33%; width: calc(100% - ( 100%/5.99999 ) ) }
    .col-7-8 { width: 87.5% }
    .col-1-8 { width: 12.5% }
    .col-3-8 { width: 37.5% }
    .col-1-3 { width: calc( 100% / 3 ) }
    .col-2-3 { width: 66.66% }

Use any combination of these in a row to create the desired layout. Only direct descendents of a `.row` will shift to 100% at the 800px breakpoint, therefore, nesting columns within columns (or other divs) will keep them at their original size. 

There are four "on/off" switch classes for the two main states: `.high-on` and `.high-off` for the high (desktop) range, and `.low-on`/`.low-off` for the lower range.

How to use Basicss
==================
The idea with OOCSS is to write rules with low specificity that can be stacked (or cascaded) on top of each other. It is like a bucket of legos for you to build things with. 

    <div class="row">
        <div class="col-1-2">
            <p class="purple px16 lh20">
                Some paragraph lorem ipsum.
            </p>
        </div>
        <div class="col-1-2">
            <div class="back-blue pad">
                <img src="path.jpg" />
            </div>
        </div>
    </div>

Scaling CSS
================
Basicss uses the scaling CSS method of keeping everything where it belongs:

- < 500px: 90% scaled (small phones)
- < 800px: 80% scaled (large handhelds)
- > 800px: 80% scaled (small desktops and horizontal handhelds)
- < 1000px: 90% scaled
- < 1100px: 100% scaled (~1024 range; horizontal ipads and average PC monitors)
- < 1200px: 110% scaled  
- ... (modern PC monitors)
- ~ 4k: 300% scaled (latest smart televisions)
