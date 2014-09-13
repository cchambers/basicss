Introduction to Basicss
=======================
Basicss is an object-oriented CSS framework; little bits of re-usable code make creating complex websites simple. The real beauty of this type of CSS is that the rules explain themselves. I will break down each group of rules that are included in the following sections.

### Changelog: 
v3 - Padding removed entirely from grid to encourage nesting. 

OOCSS
-----
### Trigger Classes 

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

These classes are generally used to preload a class with properties that will be change eventually via a JavaScript Timer or some other event on the page.

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

In regards to absolute positioning, just add the *.absolute* class and proceed to add the edge distances in-line.

    <div class="absolute back-blue" style="top:100px;left:100px"> 
        I'm absolutely positioned!
    </div>
    
#### z-index
    .sub-layer       { position: relative; z-index: -1 }
    .back-layer      { position: relative; z-index: 1 }
    .middle-layer    { position: relative; z-index: 2 }
    .front-layer     { position: relative; z-index: 3 }

### Scrollbar Control
    .overhide        { overflow: hidden }
    .overshow        { overflow: visible }
    .scroll-y        { overflow-y: scroll }

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
    .round           { border-radius: 50% }

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
    .cols2 { 
      -webkit-column-count: 2;
      -moz-column-count: 2;
      column-count: 2
    }
    .cols3 { 
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
     .px96           { font-size: 96px; font-size: 9.6rem }
     .px94           { font-size: 94px; font-size: 9.4rem }
     .px92           { font-size: 92px; font-size: 9.2rem }
     .px90           { font-size: 90px; font-size: 9.0rem }
     .px88           { font-size: 88px; font-size: 8.8rem }
     .px86           { font-size: 86px; font-size: 8.6rem }
     .px84           { font-size: 84px; font-size: 8.4rem }
     .px82           { font-size: 82px; font-size: 8.2rem }
     .px80           { font-size: 80px; font-size: 8.0rem }
     .px78           { font-size: 78px; font-size: 7.8rem }
     .px76           { font-size: 76px; font-size: 7.6rem }
     .px74           { font-size: 74px; font-size: 7.4rem }
     .px72           { font-size: 72px; font-size: 7.2rem }
     .px70           { font-size: 70px; font-size: 7.0rem }
     .px68           { font-size: 68px; font-size: 6.8rem }
     .px66           { font-size: 66px; font-size: 6.6rem }
     .px64           { font-size: 64px; font-size: 6.4rem }
     .px62           { font-size: 62px; font-size: 6.2rem }
     .px60           { font-size: 60px; font-size: 6.0rem }
     .px58           { font-size: 58px; font-size: 5.8rem }
     .px56           { font-size: 56px; font-size: 5.6rem }
     .px54           { font-size: 54px; font-size: 5.4rem }
     .px52           { font-size: 52px; font-size: 5.2rem }
     .px50           { font-size: 50px; font-size: 5.0rem }
     .px48           { font-size: 48px; font-size: 4.8rem }
     .px46           { font-size: 46px; font-size: 4.6rem }
     .px44           { font-size: 44px; font-size: 4.4rem }
     .px42           { font-size: 42px; font-size: 4.2rem }
     .px40           { font-size: 40px; font-size: 4.0rem }
     .px38           { font-size: 38px; font-size: 3.8rem }
     .px36           { font-size: 36px; font-size: 3.6rem }
     .px34           { font-size: 34px; font-size: 3.4rem }
     .px32           { font-size: 32px; font-size: 3.2rem }
     .px30           { font-size: 30px; font-size: 3.0rem }
     .px28           { font-size: 28px; font-size: 2.8rem }
     .px26           { font-size: 26px; font-size: 2.6rem }
     .px24           { font-size: 24px; font-size: 2.4rem }
     .px22           { font-size: 22px; font-size: 2.2rem }
     .px20           { font-size: 20px; font-size: 2.0rem }
     .px18           { font-size: 18px; font-size: 1.8rem }
     .px16           { font-size: 16px; font-size: 1.6rem }
     .px14           { font-size: 14px; font-size: 1.4rem }
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
    .lh96           { line-height: 96px; line-height: 9.6rem }
    .lh94           { line-height: 94px; line-height: 9.4rem }
    .lh92           { line-height: 92px; line-height: 9.2rem }
    .lh90           { line-height: 90px; line-height: 9.0rem }
    .lh88           { line-height: 88px; line-height: 8.8rem }
    .lh86           { line-height: 86px; line-height: 8.6rem }
    .lh84           { line-height: 84px; line-height: 8.4rem }
    .lh82           { line-height: 82px; line-height: 8.2rem }
    .lh80           { line-height: 80px; line-height: 8.0rem }
    .lh78           { line-height: 78px; line-height: 7.8rem }
    .lh76           { line-height: 76px; line-height: 7.6rem }
    .lh74           { line-height: 74px; line-height: 7.4rem }
    .lh72           { line-height: 72px; line-height: 7.2rem }
    .lh70           { line-height: 70px; line-height: 7.0rem }
    .lh68           { line-height: 68px; line-height: 6.8rem }
    .lh66           { line-height: 66px; line-height: 6.6rem }
    .lh64           { line-height: 64px; line-height: 6.4rem }
    .lh62           { line-height: 62px; line-height: 6.2rem }
    .lh60           { line-height: 60px; line-height: 6.0rem }
    .lh58           { line-height: 58px; line-height: 5.8rem }
    .lh56           { line-height: 56px; line-height: 5.6rem }
    .lh54           { line-height: 54px; line-height: 5.4rem }
    .lh52           { line-height: 52px; line-height: 5.2rem }
    .lh50           { line-height: 50px; line-height: 5.0rem }
    .lh48           { line-height: 48px; line-height: 4.8rem }
    .lh46           { line-height: 46px; line-height: 4.6rem }
    .lh44           { line-height: 44px; line-height: 4.4rem }
    .lh42           { line-height: 42px; line-height: 4.2rem }
    .lh40           { line-height: 40px; line-height: 4.0rem }
    .lh38           { line-height: 38px; line-height: 3.8rem }
    .lh36           { line-height: 36px; line-height: 3.6rem }
    .lh34           { line-height: 34px; line-height: 3.4rem }
    .lh32           { line-height: 32px; line-height: 3.2rem }
    .lh30           { line-height: 30px; line-height: 3.0rem }
    .lh28           { line-height: 28px; line-height: 2.8rem }
    .lh26           { line-height: 26px; line-height: 2.6rem }
    .lh24           { line-height: 24px; line-height: 2.4rem }
    .lh22           { line-height: 22px; line-height: 2.2rem }
    .lh20           { line-height: 20px; line-height: 2.0rem }
    .lh18           { line-height: 18px; line-height: 1.8rem }
    .lh16           { line-height: 16px; line-height: 1.6rem }
    .lh14           { line-height: 14px; line-height: 1.4rem }
    .lh12           { line-height: 12px; line-height: 1.2rem }
    .lh10           { line-height: 10px; line-height: 1.0rem }
    

    
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

As of version 3, this grid is no longer padded by default. Another class has been added to re-enable the default padding on a per-row basis. It has been extended to automatically pad lists and paragraphs:

    .autopad { list-style: none }
    .autopad > li { padding: 1rem 1.5rem  }
    .autopad > h2 { padding: 1.5rem 0 }
    .autopad > p {  padding-bottom: 1.5rem }
    .autopad > [class*=col-],
    .autopad-light > [class*=col-]{ padding: 3rem; padding-right: 1.5rem; padding-left: 1.5rem; }
    .autopad > [class*=col-]:first-of-type { padding-left: 3rem; }
    .autopad > [class*=col-]:last-of-type { padding-right: 3rem; }

And here is our grid:

    .row      { width: 100%; float: left }
    
    .contain{
      position: relative;
      width: 900px;
      margin: 0 auto
    }
    
    [class*=col-]{
      float: left;
      padding: 10px;
      padding-right: 30px
    }

These three elements make up our grid. Each set of columns belong in a *.row*. Any content that needs to be constrained to the center of the page is wrapped with a *.container*. 

    .col-1-1, .full   { width: 100% }
    .col-3-4          { width: 75% }
    .col-1-2, .half   { width: 50% }
    .col-1-4, .quarter{ width: 25% }
    .col-1-5, .fifth  { width: 20% }
    .col-2-5          { width: 40% }
    .col-3-5          { width: 60% }
    .col-4-5          { width: 80% }
    .col-1-8, .eighth { width: 12.5% }
    .col-1-3, .third  { width: 33.33% }
    .col-2-3          { width: 66.66% }

Super simple responsive grid. The column widths are denoted by fractions: 1-2 is 1/2, and 1-4 is 1/4, etc. You can use any combination of these to fill out a row. Careful planning with rows/columns can make transitions between breakpoints seamless.

The secondary grid definitions are not responsive to the layout... i.e, they will remain at their pre-defined width at any viewport size.

----------

There are a few abbreviated grid classes that are not affected by the media queries. They are...
    .half, .third, .qtr, .fifth

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

Notes
================
Basicss comes stock with five breakpoints:

Fluid:
 - Phones and Tablets (0 - 800px) 

Hard breakpoints for proportions: 
 - Desktops under 1000px (800px - 1000px)
 - Desktops over 1200px
 - Desktops over 1400px
 - Desktops over 1600px
 
... and two content switches...

 - .mobile
 - .desktop

... that can be used to control the visibility of different elements depending on breakpoints. An element with the ".phone" class would only show to a phone.


