Introduction to Basicss
=======================
Basicss is an object-oriented CSS framework; little bits of re-usable code make creating complex websites simple. The real beauty of this type of CSS is that the rules explain themselves. I will break down each group of rules that are included in the following sections.

OOCSS
-----
### Trigger Classes 

    .off             { display: none }
    .on              { display: block }
    .alpha-off       { opacity: 0 }
    .alpha-on        { opacity: 1 }
    .stage-right     { left: 110% !important }
    .stage-left      { right: 110% !important }
    .stage-top       { bottom: 110% !important }
    .stage-bottom    { top: 110% !important }

These classes are generally used to preload a class with properties that will be change eventually via a JavaScript Timer or some other event on the page.

### Positioning  

    .float-left      { float: left }
    .float-right     { float: right }
    .float-center    { margin-left: auto; margin-right: auto; max-width: 1020px }
    .absolute        { display: block; position: absolute }
    .inline          { display: inline-block }
    .relative        { display: block; position: relative }
    .fixed           { display: block; position: fixed }
    .static          { display: block; position: static }

In regards to absolute positioning, just add the *.absolute* class and proceed to add the edge distances in-line.

    <div class="absolute back-blue" style="top:100px;left:100px"> 
        I'm absolutely positioned!
    </div>
    
#### z-index

    .sub-layer       { z-index: -1 }
    .back-layer      { z-index: 0 }
    .middle-layer    { z-index: 5 }
    .front-layer     { z-index: 10 }

### Scrollbar Control
    .overhide        { overflow: hidden }
    .overshow        { overflow: visible }
    .scroll-y        { overflow-y: scroll }

### Box Modifications
#### Model
    .pad,
    .pad-box         { padding: 25px }
    .pad-sides       { padding-left: 25px; padding-right: 25px }
    .pad-top         { padding-top: 25px }
    .pad-bottom      { padding-bottom: 25px }
    .pad-right       { padding-right: 25px }
    .pad-left        { padding-left: 25px }
    .pad-lips        { padding-top: 25px; padding-bottom: 25px }
    .margin,
    .margin-box      { margin: 25px }
    .margin-top      { margin-top: 25px }
    .margin-bottom   { margin-bottom: 25px }
    .margin-right    { margin-right: 25px }
    .margin-left     { margin-left: 25px }
    .margin-sides    { margin-left: 25px; margin-right: 25px }
    .margin-lips     { margin-top: 25px; margin-bottom: 25px }
    .pull-top        { margin-top: -25px }
    .pull-bottom     { margin-bottom: -25px }
    .pull-right      { margin-right: -25px }
    .pull-left       { margin-left: -25px }
    .pull-top-hard   { margin-top: -50px }
    .pull-bottom-hard{ margin-bottom: -50px }
    .pull-right-hard { margin-right: -50px }
    .pull-left-hard  { margin-left: -50px }
    .round           { border-radius: 50% }


#### Background
    .back-purple     { background: #650360 }
    .back-violet     { background: #4A0246 }
    .back-blue       { background: #328FC2 }
    .back-cyan       { background: #8BD3F5 }
    .back-sand       { background: #E8D4A3 }
    .back-toaster    { background: #5EADB2 }
    .back-steel      { background: #C0D0D8 }
    .back-dark-steel { background: #86B1C5 }
    .back-dark-blue  { background: #006899 }
    .back-white      { background: #F2F2F2 }
    .back-light-gray { background: #F4F4F4 }
    .back-gray       { background: #EEEEEE }
    .back-grayer     { background: #999999 }
    .back-dark-gray  { background: #505050 }
    .back-account1   { background: #00A4D9 }
    .back-account2   { background: #333093 }
    .back-account3   { background: #A54399 }
    .back-account4   { background: #00B273 }
    .back-error      { background: #990000 }
    .back-success    { background: #2F7215 }

### Text Modifications  
#### Weights

    .ultralight{
      font-family: 'HelveticaNeue-UltraLight',
        'Helvetica Neue UltraLight',
        'Helvetica Neue', 
        Helvetica, Arial, Roboto, sans-serif;
         font-weight: 100;
         letter-spacing: 1px
    }
    .light   { 
       font-family: "HelveticaNeue-Light", 
         "Helvetica Neue Light", 
        Helvetica, Arial, Roboto, sans-serif }
    .normal  {
       font-family: "Helvetica Neue", 
        Helvetica, Arial, Roboto, sans-serif;
       font-weight: normal }
    .bold    {
       font-family: "Helvetica Neue", 
        Helvetica, Arial, Roboto, sans-serif;
       font-weight: 700 }
    
#### Alignment
    .text-right     { text-align: right }
    .text-left      { text-align: left }
    .text-center    { text-align: center }
    .text-justify   { text-align: justify }
    
#### Size
    .px50           { font-size: 50px }
    .px48           { font-size: 48px }
    .px46           { font-size: 46px }
    .px44           { font-size: 44px }
    .px42           { font-size: 42px }
    .px40           { font-size: 40px }
    .px38           { font-size: 38px }
    .px36           { font-size: 36px }
    .px34           { font-size: 34px }
    .px32           { font-size: 32px }
    .px30           { font-size: 30px }
    .px28           { font-size: 28px }
    .px26           { font-size: 26px }
    .px24           { font-size: 24px }
    .px22           { font-size: 22px }
    .px20           { font-size: 20px }
    .px18           { font-size: 18px }
    .px16           { font-size: 16px }
    .px14           { font-size: 14px }
    .px12           { font-size: 12px }
    .px10           { font-size: 10px }
    
#### Case
    .normalcase     { text-transform: normal }
    .uppercase      { text-transform: uppercase }
    .lowercase      { text-transform: lowercase }
    .titlecase      { text-transform: capitalize }
    .strike         { text-decoration: line-through }

#### Line Height    
    .lh50           { line-height: 50px }
    .lh48           { line-height: 48px }
    .lh46           { line-height: 46px }
    .lh44           { line-height: 44px }
    .lh42           { line-height: 42px }
    .lh40           { line-height: 40px }
    .lh38           { line-height: 38px }
    .lh36           { line-height: 36px }
    .lh34           { line-height: 34px }
    .lh32           { line-height: 32px }
    .lh30           { line-height: 30px }
    .lh28           { line-height: 28px }
    .lh26           { line-height: 26px }
    .lh24           { line-height: 24px }
    .lh22           { line-height: 22px }
    .lh20           { line-height: 20px }
    .lh18           { line-height: 18px }
    .lh16           { line-height: 16px }
    .lh14           { line-height: 14px }
    .lh12           { line-height: 12px }
    .lh10           { line-height: 10px }
    

#### Colors
    .purple         { color: #650360 }
    .violet         { color: #4A0246 }
    .blue           { color: #328FC2 }
    .cyan           { color: #8BD3F5 }
    .sand           { color: #E8D4A3 }
    .toaster        { color: #5EADB2 }
    .steel          { color: #C0D0D8 }
    .dark-steel     { color: #86B1C5 }
    .dark-blue      { color: #006899 }
    .white          { color: #F2F2F2 }
    .light-gray     { color: #F4F4F4 }
    .gray           { color: #EEEEEE }
    .grayer         { color: #999999 }
    .dark-gray      { color: #505050 }
    .account1       { color: #00A4D9 }
    .account2       { color: #333093 }
    .account3       { color: #A54399 }
    .account4       { color: #00B273 }
    .error          { color: #990000 }
    .success        { color: #2F7215 }
    

    
Flexbox 
-------
Flexbox is supported in most modern browsers, but implemented in too many ways to even try to remember.

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
     
The *.flex* class can be applied to any container to make the children capable of becoming flex-items. The default settings above make items justify themselves across a single row, but there are a number of class mods that can be applied...
     
#### Flex Container Modifications
    .flex.row        { flex-direction: row; -ms-flex-direction: row }
    .flex.row-rev    { flex-direction: row-reverse; -ms-flex-direction: row-reverse }
    .flex.col        { flex-direction: column; -ms-flex-direction: column }
    .flex.col-rev    { flex-direction: column-reverse; -ms-flex-direction: column-reverse }
Flex-items can be displayed as rows or columns, and even reversed. 

    .flex.wrap       { flex-wrap: wrap; -ms-flex-wrap: wrap }
    .flex.nowrap     { flex-wrap: nowrap; -ms-flex-wrap: nowrap }
    .flex.wrap-rev   { flex-wrap: wrap-reverse; -ms-flex-wrap: wrap-reverse }
The default setting is "nowrap", but if you want your elements to break to another line, you will need to change this by adding a *.wrap*.
    
    .flex.start      { justify-content: flex-start; -ms-flex-pack: start }
    .flex.end        { justify-content: flex-end; -ms-flex-pack: end }
    .flex.center     { justify-content: center; -ms-flex-pack: center }
    .flex.between    { justify-content: space-between; -ms-flex-pack: justify }
    .flex.around     { justify-content: space-around; -ms-flex-pack: justify }

    .flex.top        { align-content: flex-start; -ms-flex-align: start }
    .flex.bottom     { align-content: flex-end; -ms-flex-align: end }
    .flex.middle     { align-content: center; -ms-flex-align: center }
    .flex.fill       { align-content: stretch; -ms-flex-align: stretch }
    .flex.content    { align-content: baseline; -ms-flex-align: baseline }


### Flex Item
    .flex-item {
       flex-grow: 0;
       flex-shrink:.5;
       flex-basis: auto
     }
     
#### Flex Item Modifications
    
    .flex-item.single  { flex-grow: 0 }
    .flex-item.double  { flex-grow: 1 }
    .flex-item.triple  { flex-grow: 2 }
Flex items are allowed to grow relative to their width. So, a *.single* with a width setting of 200px would grow no larger than 200px, while a *.double* flex-item could grow to 400px, etc.
    
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

**Pro-tip:** You can force an element to the front indefinitely by giving it a negative order.

Responsive Grid
---------------

    .row      { width: 100%; float: left }
    
    .contain{
      position: relative;
      width: 900px;
      margin: 0 auto
    }
    
    [class*=col-]{
      float: left;
      padding: 10px;
      padding-right: 25px
    }

These three elements make up our grid. Each set of columns belong in a *.row*. Any content that needs to be constrained to the center of the page is wrapped with a *.container*. 
    
    .row:after,
    .contain:after,
    [class*=col-]:after{ content: "."; display: block; height: 0; overflow: hidden }

This group of rules add an extra line to every one of grid elements that acts as a float "clear fix", eliminating the need of an extra div to clear floats.  

    .col-1-1        { width: 100% }
    .col-3-4        { width: 75% }
    .col-1-2        { width: 50% }
    .col-1-4        { width: 25% }
    .col-1-8        { width: 12.5% }
    .col-1-16       { width: 6.25% }
    .col-2-3        { width: 66.66% }
    .col-1-3        { width: 33.33% }

Super simple responsive grid. The column widths are denoted by fractions: 1-2 is 1/2, and 1-4 is 1/4, etc. You can use any combination of these to fill out a row. Careful planning with rows/columns can make transitions between breakpoints seamless.

----------

How to use Basicss
==================
The idea with OOCSS is to write rules with low specificity that can be stacked (or cascaded) on top of each other. It is like having a pantry full of ingredients and the recipe is up to you. 

    <div class="row px16 lh20">
        <div class="col-1-2">
            <p class="purple">
                Some paragraph lorem ipsum.
            </p>
        </div>
        <div class="col-1-2 back-blue pad">
            <img src="path.jpg" />
        </div>
    </div>

Form Fields
-----------
Forms are handled the same way they always have been, but instead of using a form element, we use a .form wrapper which can be applied directly to the grid:

    <div class="row form">
        <div class="col-1-4">
            <label for="username req">
                Username
            </label>
        </div>
        
        <div class="col-1-4">
            <input id="username" placeholder="username" />
        </div>
    </div>
    
----------

Notes
================
Basicss comes stock with 4 breakpoints...

 - Phones only (0 - 500px)
 - Phones and Tablets (0 - 768px) 
 - Desktops under 1020px (768px - 1020px)
 - Desktops over 1020px
 
... and three content switches...

 - .phone
 - .tablet
 - .desktop

... that can be used to control the visibility of different elements depending on breakpoints. An element with the ".phone" class would only show to a phone.


