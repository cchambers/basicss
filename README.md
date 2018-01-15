Introduction
=======================
Basicss is an object-oriented scaling CSS framework. The real beauty of OO CSS is that the classes explain themselves. I will break down each group of rules that are included in the following sections...

### Major Change Log: 
- v3 - Padding removed entirely from content flow system to encourage nesting.  
- v3.4.5 - Added portrait orientation to "touch" breakpoint.  
- v4 - "desktop" and "touch" deprecated - replaced with "high-on/high-off" and "low-on/low-off".  
- v5 - Rows now use flex; items outside of rows still use float... you won't notice much of a difference.  
        - Removed pixel definitons to lower file size.  
        - Deprecated classes removed.  
        - OO classes are becoming the norm so we have simplified a bunch of class names:  
          - "lips" -> y  
          - "sides" -> x  
          - "light" -> half  
          - "hard" -> double  
          - "super" -> quad  

OOCSS
-----
### Box Modifications
#### Model
    .pad{-edge}{-amount}
    .margin{-edge}{-amount}

    Edges: t, r, b, l, x (l+r), y (t+b)
    Amounts: half, [none], double, quad

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
    .force-justify:after {
      display: inline-block;
      width: 100%;
      content: '.';
      height: 0;
      overflow: hidden;
    }
    
#### Size
    .px100          { font-size: 10rem }
    .px98           { font-size: 9.8rem }
    ...
    .px12           { font-size: 1.2rem }
    .px10           { font-size: 1.0rem }
    
#### Case
    .normalcase     { text-transform: normal }
    .uppercase      { text-transform: uppercase }
    .lowercase      { text-transform: lowercase }
    .titlecase      { text-transform: capitalize }
    .strike         { text-decoration: line-through }
    .italic         { font-style: italic }

#### Line Height    
    .lh100          { line-height: 10rem }
    .lh98           { line-height: 9.8rem }
    ...
    .lh12           { line-height: 1.2rem }
    .lh10           { line-height: 1.0rem }


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
    .bottom-layer    { position: relative; z-index: 1 }
    .middle-layer    { position: relative; z-index: 2 }
    .top-layer       { position: relative; z-index: 3 }
    
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
       display: flex;
       flex-direction: row;
       flex-wrap: nowrap;
       justify-content: space-between;
     }
     
The `.flex` class can be applied to any container to make the children capable of becoming flex-items. The default settings above make items justify themselves across a single row, but there are a number of class mods that can be applied...
     
#### Flex Container Modifications
    .flex.row        { flex-direction: row }
    .flex.row-rev    { flex-direction: row-reverse }
    .flex.col        { flex-direction: column}
    .flex.col-rev    { flex-direction: column-reverse }
    
Flex-items can be displayed as rows or columns, and even reversed. 

    .flex.wrap       { flex-wrap: wrap }
    .flex.nowrap     { flex-wrap: nowrap }
    .flex.wrap-rev   { flex-wrap: wrap-reverse; }
    
The default setting is "nowrap", but if you want your elements to break to another line, you will need to change this by adding a `.wrap`.
    
    .flex.start      { justify-content: flex-start }
    .flex.end        { justify-content: flex-end }
    .flex.center     { justify-content: center }
    .flex.between    { justify-content: space-between }
    .flex.around     { justify-content: space-around }

    .flex.top        { align-content: flex-start }
    .flex.bottom     { align-content: flex-end }
    .flex.middle     { align-content: center }
    .flex.stretch    { align-content: stretch }
    .flex.content    { align-content: baseline }

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

Flex items are allowed to grow relative to their width. A `.single` item with a width setting of 200px would grow no larger than 200px, while a `.double` flex-item could grow to 400px, etc.
    
    .order-0{ order: 0 }
    .order-1{ order: 1 }
    .order-2{ order: 2 }
    .order-3{ order: 3 }
    .order-4{ order: 4 }
    .order-5{ order: 5 }
    .order-6{ order: 6 }
    .order-7{ order: 7 }
    .order-8{ order: 8 }
    .order-9{ order: 9 }
    
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

There are four "on/off" switch classes for the two main states: `.high-on`/`.high-off` for the high (desktop) range, and `.low-on`/`.low-off` for the lower range.

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
- ~ 4k: 300% scaled 
