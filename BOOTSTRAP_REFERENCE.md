# Bootstrap 5 Quick Reference Guide

## Layout & Grid System

### Containers
```html
<div class="container">      <!-- Fixed-width, responsive -->
<div class="container-fluid"> <!-- Full-width -->
```

### Grid System
```html
<div class="row">
    <div class="col">         <!-- Equal width -->
    <div class="col-6">       <!-- 6/12 width -->
    <div class="col-md-4">    <!-- 4/12 on medium+ screens -->
</div>
```

### Responsive Breakpoints
- `col-` - Extra small (< 576px)
- `col-sm-` - Small (≥ 576px)
- `col-md-` - Medium (≥ 768px)
- `col-lg-` - Large (≥ 992px)
- `col-xl-` - Extra large (≥ 1200px)
- `col-xxl-` - Extra extra large (≥ 1400px)

## Typography

### Headings
```html
<h1 class="h1">Heading 1</h1>
<p class="h2">Paragraph as heading 2</p>
```

### Display Headings
```html
<h1 class="display-1">Large display</h1>
<h1 class="display-6">Small display</h1>
```

## Components

### Cards
```html
<div class="card">
    <img class="card-img-top" src="...">
    <div class="card-body">
        <h5 class="card-title">Title</h5>
        <p class="card-text">Content</p>
        <a href="#" class="btn btn-primary">Button</a>
    </div>
</div>
```

### Navigation
```html
<nav class="navbar navbar-expand-lg">
    <ul class="nav">
        <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
        </li>
    </ul>
</nav>
```

### Navbar (Responsive)
```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Brand</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarsExample" aria-controls="navbarsExample" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarsExample">
      <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
        <li class="nav-item"><a class="nav-link active" aria-current="page" href="#">Home</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Features</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Pricing</a></li>
      </ul>
    </div>
  </div>
  <!-- requires navbar-light + navbar-toggler-icon CSS from Bootstrap -->
  <!-- include bundle JS for collapse to work -->
  <!-- <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js"></script> -->
```

### Forms
```html
<div class="mb-3">
    <label class="form-label">Label</label>
    <input type="text" class="form-control">
</div>
<div class="form-check">
    <input class="form-check-input" type="checkbox">
    <label class="form-check-label">Checkbox</label>
</div>
```

### Buttons
```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-danger">Danger</button>
```

### Button Sizes and Groups
```html
<button class="btn btn-primary btn-sm">Small</button>
<button class="btn btn-primary">Default</button>
<button class="btn btn-primary btn-lg">Large</button>

<div class="btn-group" role="group">
  <button type="button" class="btn btn-outline-secondary">Left</button>
  <button type="button" class="btn btn-outline-secondary">Middle</button>
  <button type="button" class="btn btn-outline-secondary">Right</button>
  </div>
```

## Spacing Utilities

### Padding
- `p-{0-5}` - All sides
- `pt-{0-5}` - Top
- `pb-{0-5}` - Bottom
- `ps-{0-5}` - Start (left)
- `pe-{0-5}` - End (right)
- `px-{0-5}` - Horizontal (left & right)
- `py-{0-5}` - Vertical (top & bottom)

### Margin
- `m-{0-5}` - All sides
- `mt-{0-5}` - Top
- `mb-{0-5}` - Bottom
- `ms-{0-5}` - Start (left)
- `me-{0-5}` - End (right)
- `mx-{0-5}` - Horizontal (left & right)
- `my-{0-5}` - Vertical (top & bottom)

### Spacing Scale
- `0` = 0rem
- `1` = 0.25rem (4px)
- `2` = 0.5rem (8px)
- `3` = 1rem (16px)
- `4` = 1.5rem (24px)
- `5` = 3rem (48px)

## Colors

### Background Colors
```html
<div class="bg-primary">Primary</div>
<div class="bg-secondary">Secondary</div>
<div class="bg-success">Success</div>
<div class="bg-danger">Danger</div>
<div class="bg-warning">Warning</div>
<div class="bg-info">Info</div>
<div class="bg-light">Light</div>
<div class="bg-dark">Dark</div>
<div class="bg-white">White</div>
```

### Text Colors
```html
<p class="text-primary">Primary text</p>
<p class="text-white">White text</p>
<p class="text-dark">Dark text</p>
```

## Flexbox Utilities

### Display
```html
<div class="d-flex">Flexbox container</div>
<div class="d-inline-flex">Inline flexbox</div>
```

### Direction
```html
<div class="flex-row">Row (default)</div>
<div class="flex-column">Column</div>
```

### Justify Content (horizontal alignment)
```html
<div class="justify-content-start">Start</div>
<div class="justify-content-center">Center</div>
<div class="justify-content-end">End</div>
<div class="justify-content-between">Space between</div>
<div class="justify-content-around">Space around</div>
```

### Align Items (vertical alignment)
```html
<div class="align-items-start">Start</div>
<div class="align-items-center">Center</div>
<div class="align-items-end">End</div>
```

## Images

### Responsive Images
```html
<img class="img-fluid" src="...">     <!-- Responsive -->
<img class="img-thumbnail" src="..."> <!-- Thumbnail border -->
```

### Image Shapes
```html
<img class="rounded" src="...">        <!-- Rounded corners -->
<img class="rounded-circle" src="..."> <!-- Circle -->
```

## Position & Display

### Position
```html
<div class="position-static">Static</div>
<div class="position-relative">Relative</div>
<div class="position-absolute">Absolute</div>
<div class="position-fixed">Fixed</div>
<div class="sticky-top">Sticky top</div>
```

### Display
```html
<div class="d-none">Hidden</div>
<div class="d-block">Block</div>
<div class="d-inline">Inline</div>
<div class="d-inline-block">Inline block</div>
```

### Responsive Display
```html
<div class="d-none d-md-block">Hidden on small, visible on medium+</div>
<div class="d-block d-md-none">Visible on small, hidden on medium+</div>
```

## Borders

### Border
```html
<div class="border">All borders</div>
<div class="border-top">Top border</div>
<div class="border-0">No border</div>
```

### Border Colors
```html
<div class="border border-primary">Primary border</div>
<div class="border border-success">Success border</div>
```

## Text Utilities

### Text Alignment
```html
<p class="text-start">Left aligned</p>
<p class="text-center">Center aligned</p>
<p class="text-end">Right aligned</p>
```

### Text Transform
```html
<p class="text-lowercase">lowercase</p>
<p class="text-uppercase">UPPERCASE</p>
<p class="text-capitalize">Capitalize</p>
```

### Font Weight
```html
<p class="fw-bold">Bold text</p>
<p class="fw-normal">Normal weight</p>
<p class="fw-light">Light weight</p>
```

## Sizing

### Width
```html
<div class="w-25">25% width</div>
<div class="w-50">50% width</div>
<div class="w-75">75% width</div>
<div class="w-100">100% width</div>
```

### Height
```html
<div class="h-25">25% height</div>
<div class="h-50">50% height</div>
<div class="h-75">75% height</div>
<div class="h-100">100% height</div>
```

## Common Patterns from Your Code

### Responsive Card Grid
```html
<div class="container-fluid">
    <div class="row g-4 p-4">
        <div class="col-12 col-md-4 col-lg-3 col-sm-6">
            <div class="card">
                <!-- Card content -->
            </div>
        </div>
    </div>
</div>
```

### Sticky Navigation
```html
<header class="sticky-top">
    <div class="navbar bg-light px-3">
        <div class="col">
            <h1>Logo</h1>
        </div>
        <div class="col">
            <ul class="nav d-flex flex-row justify-content-end">
                <!-- Nav items -->
            </ul>
        </div>
    </div>
</header>
```

### List Group
```html
<ul class="list-group">
  <li class="list-group-item">An item</li>
  <li class="list-group-item list-group-item-primary">A primary item</li>
  <li class="list-group-item list-group-item-action">Clickable item</li>
  <li class="list-group-item disabled">Disabled item</li>
 </ul>
```

### Tooltips (init required)
```html
<button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" title="Tooltip text">Hover me</button>
<script>
  const tooltipTriggerList = Array.from(document.querySelectorAll('[data-bs-toggle="tooltip"]'));
  tooltipTriggerList.forEach(el => new bootstrap.Tooltip(el));
 </script>
```

### Toasts
```html
<div class="toast" role="alert" aria-live="assertive" aria-atomic="true" data-bs-delay="2000">
  <div class="toast-header">
    <strong class="me-auto">Notice</strong>
    <button type="button" class="btn-close" data-bs-dismiss="toast" aria-label="Close"></button>
  </div>
  <div class="toast-body">Hello, world!</div>
 </div>
<script>
  const toastEl = document.querySelector('.toast');
  new bootstrap.Toast(toastEl).show();
 </script>
```

### Carousel
```html
<div id="demoCarousel" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active"><img src="images/image-30914.jpg" class="d-block w-100" alt="..."></div>
    <div class="carousel-item"><img src="images/image-33330.jpg" class="d-block w-100" alt="..."></div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#demoCarousel" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#demoCarousel" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
 </div>
```

### Modal (Popup)
```html
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">Launch Modal</button>
<div class="modal fade" id="exampleModal" tabindex="-1" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Modal title</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">Modal body text</div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div>
    </div>
  </div>
 </div>
```

### Accordion
```html
<div class="accordion" id="accordionExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">Item #1</button>
    </h2>
    <div id="collapseOne" class="accordion-collapse collapse show" data-bs-parent="#accordionExample">
      <div class="accordion-body">Content for item #1</div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">Item #2</button>
    </h2>
    <div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
      <div class="accordion-body">Content for item #2</div>
    </div>
  </div>
 </div>
```

### Centered Form
```html
<form class="p-4 d-flex justify-content-center bg-dark">
    <div class="col-12 col-md-6 col-lg-4 border p-2 text-white">
        <!-- Form fields -->
    </div>
</form>
```

### Horizontal Card Layout
```html
<div class="card">
    <div class="row">
        <div class="col-6 col-sm-12">
            <img class="img-fluid rounded h-100 w-100" src="...">
        </div>
        <div class="col-6 col-sm-12">
            <div class="card-body">
                <!-- Content -->
            </div>
        </div>
    </div>
</div>
```

## CDN Links (Bootstrap 5.0.2)

### CSS
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" 
      rel="stylesheet" 
      integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" 
      crossorigin="anonymous">
```

### JavaScript
```html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" 
        integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" 
        crossorigin="anonymous"></script>
```

### Required Meta Tag
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
