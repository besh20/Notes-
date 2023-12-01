# CSS Bootstrap

- **Bootstrap Containers;**
    
    Containers are the most basic layout element in Bootstrap and are required when using the grid system. Containers are basically used to wrap content with some padding. They are also used to align the content horizontally center on the page in case of fixed width layout.
    
    Bootstrap provides three different types containers:
    
    - `.container`, which has a max-width at each responsive breakpoint.
    - `.container-fluid`, which has 100% width at all breakpoints.
    - `.container-{breakpoint}`, which has 100% width until the specified breakpoint.
    
    | ClassesBootstrap  Grid System | X-Small<576px | Small≥576px | Medium≥768px | Large≥992px | X-Large≥1200px | XX-Large≥1400px |
    | --- | --- | --- | --- | --- | --- | --- |
    | .container | 100% | 540px | 720px | 960px | 1140px | 1320px |
    | .container-sm | 100% | 540px | 720px | 960px | 1140px | 1320px |
    | .container-md | 100% | 100% | 720px | 960px | 1140px | 1320px |
    | .container-lg | 100% | 100% | 100% | 960px | 1140px | 1320px |
    | .container-xl | 100% | 100% | 100% | 100% | 1140px | 1320px |
    | .container-xxl | 100% | 100% | 100% | 100% | 100% | 1320px |
    | .container-fluid | 100% | 100% | 100% | 100% | 100% | 100% |

### **Bootstrap grid-system**

 ****Bootstrap’s grid system uses a series of containers, rows, and columns to layout and align content. It’s built with [flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox) and is fully responsive. Below is an example and an in-depth explanation for how the grid system comes together.

Bootstrap grid system provides an easy and powerful way to create responsive layouts of all shapes and sizes. It is built with [flexbox](https://www.tutorialrepublic.com/css-tutorial/css3-flexible-box-layouts.php) with mobile-first approach. Also, it is fully responsive and uses twelve column system (12 columns available per row) and six default responsive tiers.

### **Offsetting the Grid Columns**

You can also move grid columns to the right for alignment purpose using the column offset classes like `.offset-sm-*`, `.offset-md-*`, `.offset-lg-*`, and so on.

### **Creating Compact Columns**

You can remove the default gutters between columns to create compact layouts by adding the class `.g-0` on `.row`. This class removes the negative margins from row and the horizontal padding from all immediate children columns.

### **Reordering of Grid Columns**

You can even change the visual order of your grid columns without changing their order in actual markup. Use the class `.order-last` to order the column in last, whereas use the class `.order-first` to order the column at first place.

### **Breaking Columns to a New Line**

You can also create equal-width columns that span multiple rows by inserting a `<div>` with `.w-100` class where you want the columns to break to a new line. Additionally, you can make these breaks responsive by combining the `.w-100`

| xs<576px | sm≥576px | md≥768px | lg≥992px | xl≥1200px | xxl≥1400px |
| --- | --- | --- | --- | --- | --- |
| Container max-width | None (auto) | 540px | 720px | 960px | 1140px |
| Class prefix | .col- | .col-sm- | .col-md- | .col-lg- | .col-xl- |
| # of columns | 12 |  |  |  |  |
| Gutter width | 1.5rem (.75rem on left and right) |  |  |  |  |
| Custom gutters | https://getbootstrap.com/docs/5.3/layout/gutters/ |  |  |  |  |
| Nestable | https://getbootstrap.com/docs/5.3/layout/grid/#nesting |  |  |  |  |
| Column ordering | https://getbootstrap.com/docs/5.3/layout/columns/#reordering |  |  |  |  |

```html
<div class="container">
    <!--Row with two equal columns-->
    <div class="row">
        <div class="col-md-6">Column left</div>
        <div class="col-md-6">Column right</div>
    </div>
    
    <!--Row with two columns divided in 1:2 ratio-->
    <div class="row">
        <div class="col-md-4">Column left</div>
        <div class="col-md-8">Column right</div>
    </div>
    
    <!--Row with two columns divided in 1:3 ratio-->
    <div class="row">
        <div class="col-md-3">Column left</div>
        <div class="col-md-9">Column right</div>
    </div>
</div>
```

### ****Buttons****

```html
<button type="button" class="btn btn-outline-primary">Primary</button>
<button type="button" class="btn btn-outline-secondary">Secondary</button>
<button type="button" class="btn btn-outline-success">Success</button>
<button type="button" class="btn btn-outline-danger">Danger</button>
<button type="button" class="btn btn-outline-warning">Warning</button>
<button type="button" class="btn btn-outline-info">Info</button>
<button type="button" class="btn btn-outline-light">Light</button>
<button type="button" class="btn btn-outline-dark">Dark</button>
```

### Cards

A **card** is a flexible and extensible content container. It includes options for headers and footers, a wide variety of content, contextual background colors, and powerful display options. If you’re familiar with Bootstrap 3, cards replace our old panels, wells, and thumbnails. Similar functionality to those components is available as modifier classes for cards.

```html
<div class="card" style="width: 18rem;">
  <img src="..." class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

****Navbar****

## **Supported content**

Navbars come with built-in support for a handful of sub-components. Choose from the following as needed:

- `.navbar-brand` for your company, product, or project name.
- `.navbar-nav` for a full-height and lightweight navigation (including support for dropdowns).
- `.navbar-toggler` for use with our collapse plugin and other [navigation toggling](https://getbootstrap.com/docs/5.3/components/navbar/#responsive-behaviors) behaviors.
- Flex and spacing utilities for any form controls and actions.
- `.navbar-text` for adding vertically centered strings of text.
- `.collapse.navbar-collapse` for grouping and hiding navbar contents by a parent breakpoint.
- Add an optional `.navbar-scroll` to set a `max-height` and [scroll expanded navbar content](https://getbootstrap.com/docs/5.3/components/navbar/#scrolling).

```html
<nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Dropdown
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
```