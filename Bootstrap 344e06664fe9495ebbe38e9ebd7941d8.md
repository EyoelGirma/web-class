# Bootstrap

# What Is Bootstrap?

Bootstrap is an open source product from Mark Otto and Jacob Thornton who, when
it was initially released, were both employees at Twitter. There was a need to standardize
the frontend toolsets of engineers across the company.

It was released as an open source product in August 2011 on GitHub

One of the problem with basic HTML design is that the webpage may look different in different browser or device (e.g. mobile, tablet and laptop). Therefore, we may need to modify the code according to browser or device. The problem can be easily resolved by using Bootstrap.

Bootstrap is a framework which uses HTML, CSS and JavaScript for the web design. It is supported by all the major browsers e.g. Firefox, Opera and Chrome etc. Further, Bootstrap includes several predefined classes for easy layouts e.g. dropdown buttons, navigation bar and alerts etc. Lastly, it is responsive in nature i.e. the layout changes automatically according to the device e.g. mobile or laptop etc.

### Why Use Bootstrap?

Advantages of Bootstrap:

- **Easy to use**: Anybody with just basic knowledge of HTML and CSS can start using Bootstrap
- **Responsive features**: Bootstrap's responsive CSS adjusts to phones, tablets, and desktops
- **Mobile-first approach**: In Bootstrap 3, mobile-first styles are part of the core framework
- **Browser compatibility**: Bootstrap is compatible with all modern browsers (Chrome, Firefox, Internet Explorer, Edge, Safari, and Opera

### Bootstrap File Structure

bootstrap/
├── css/
│ ├── bootstrap.css
│ ├── bootstrap.min.css
├── js/
│ ├── bootstrap.js
│ ├── bootstrap.min.js
├── img/
│ ├── glyphicons-halflings.png
│ ├── glyphicons-halflings-white.png
└── [README.md](http://readme.md/)
The Bootstrap download includes three folders: css, js, and img. For simplicity, add these
to the root of your project. Minified versions of the CSS and JavaScript are also included.
It is not necessary to include both the uncompressed and the minified versions. For the
sake of brevity, I use the uncompressed version during development and then switch to
the compressed version in production.

### What Bootstrap Package Includes?

1. Scaffolding: Bootstrap provides a basic structure with Grid System, link styles, background. This is is
covered in detail in the section Bootstrap Basic Structure
2. CSS: Bootstrap comes with feature of global CSS settings, fundamental HTML elements styled and enhanced with extensible classes, and an advanced grid system. This is covered in detail in the section Bootstrap with CSS.
3.  Components: Bootstrap contains over a dozen reusable components built to provide iconography, dropdowns, navigation, alerts, popovers, and much more. This is covered in detail in the section Layout Components.
4. JavaScript Plugins: Bootstrap contains over a dozen custom jQuery plugins. You can easily include them xall, or one by one. This is covered in details in the section Bootstrap Plugins.
5. Customize: You can customize Bootstrap's components, LESS variables, and jQuery plugins to get your very own version.

### Setup

Bootstrap needs at least 3 files for its operation which can be downloaded from the Bootstrap website.
• bootstrap.css : This file contains various CSS for bootstrap.
• bootstrap.js : This file contains various JavaScript functionalities e.g. dropdown and alerts etc.
• jQuery.js : This file is the jQuery library which can be downloaded from the ‘jQuery’ website. It is required for proper working of ‘bootstrap.js’.

### Download and include files

<!DOCTYPE html>
 <html>
 <head>
 <title>Bootstrap Tutorial</title>
 <!-- CSS -->
 <link href="asset/css/bootstrap.min.css" rel="stylesheet">
 <!-- Add Custom CSS below -->
 </head>
 <body>
 <!-- Javascript -->
 <!-- put jQuery.js before bootstrap.min.js; and then add custom jquery -->

<script src="asset/js/jquery-3.3.1.min.js"></script>
 <script src="asset/js/bootstrap.min.js"></script>
 </body>
 </html>

### **Containers**

Containers are a fundamental building block of Bootstrap that contain, pad, and align your content within a given device or viewport.

Bootstrap comes with three different containers:

- `.container`, which sets a `max-width` at each responsive breakpoint
- `.container-fluid`, which is `width: 100%` at all breakpoints
- `.container-{breakpoint}`, which is `width: 100%` until the specified breakpoint

for example:

- **Extra small (**<576px)
- *Small (**≥576px)
- *Medium (**≥768px)
- *Large (**≥992px)
- *X-Large (**≥1200px)
- *XX-Large (**≥1400px)

## Bootstrap Grid System

### What is a Grid?

As put by Wikipedia: In graphic design, a grid is a structure (usually two-dimensional) made up of a series of intersecting straight (vertical, horizontal) lines used to structure content. It is widely used to design layout and content structure in print design. In web design, it is a very effective method to create a consistent layout rapidly and effectively using HTML and CSS. To put it simple words grids in web design organise and structure content, makes websites easy to scan and reduces cognitive load on users.

**What is Bootstrap Grid System?**

As put by the official documentation of Bootstrap for grid system:
Bootstrap includes a responsive, mobile first fluid grid system that appropriately scales up to 12 columns as the device or viewport size increases. It includes predefined classes for easy layout options, as well as powerful mixins for generating more semantic layouts.

<div class="container text-center">
  <div class="row">
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
  </div>
</div>

The above example creates three equal-width columns across all devices and viewports using our predefined grid classes. Those columns are centered in the page with the parent `.container`.

Let us understand the above statement. Bootstrap 3 is mobile first in the sense that the code for Bootstrap now starts by targeting smaller screens like mobile devices, tablets, and then “expands” components and grids for larger screens such as laptops, desktops.

MOBILE FIRST STRATEGY
* Content
       - Determine what is most important.
* Layout
       - Design to smaller widths first

       - Base CSS address mobile device first; media queries address for tablet, desktops.
* Progressive Enhancement
        - Add elements as screen size increases.

**Working of Bootstrap Grid System**
Grid systems are used for creating page layouts through a series of rows and columns that house your content. Here's how the Bootstrap grid system works:
* Rows must be placed within a .container class for proper alignment and padding.
* Use rows to create horizontal groups of columns.
* Content should be placed within columns, and only columns may be immediate children of rows.
* Predefined grid classes like .row and .col-xs-4 are available for quickly making grid layouts. LESS mixins can also be used for more semantic layouts.
* Columns create gutters (gaps between column content) via padding. That padding is offset in rows for the first and last column via negative margin on .rows.
* Grid columns are created by specifying the number of twelve available columns you wish to span. For example, three equal columns would use three .col-xs-4.

### Navbar

The navbar is a nice feature, and is one of the prominent features of Bootstrap sites (see
Figure 3-22). At its core, the navbar includes styling for site names and basic navigation.
It can later be extended by adding form-specific controls and specialized dropdowns.
To be sure that the navbar is constrained to the width of the content of the page, either
place it inside of a .span12 or the .container class:

[Title](notion://www.notion.so/Bootstrap-344e06664fe9495ebbe38e9ebd7941d8#)

```jsx
<div class="navbar">
 <div class="navbar-inner">
 <a class="brand" href="#">Title</a>
 <ul class="nav">
 <li class="active"><a href="#">Home</a></li>
 <li><a href="#">Link</a></li>
 <li><a href="#">Link</a></li>
 </ul>
 </div>
</div>
```