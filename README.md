# responsive-portfolio

This is homework assignment #2: Responsive Portfolio. In this assignment, we, the students of Fullstack Web Development, were tasked to create a responsive website using bootstrap. There were 3 main breaking points assigned and referenced in the assets folder that we had to follow: 980px (desktop), 768px (tablet), and 640px (mobile). The task assigned was to follow the reference pictures in the assets folder and do our best to re-create or make something similar to the designs assigned.
 
 ## Getting Started

* Create the following files files: `index.html`, `portfolio.html` and `contact.html`.

* Using Bootstrap, develop your portfolio site with the following items:

   * A navbar

   * A responsive layout

   * Responsive images

* The Bootstrap portfolio should minimize the use of media queries.

* Screenshots are provided as a reference in the `Assets/Images` folder. Your app does not need to be _exactly_ like the images. Use Bootstrap to create a similar, responsive layout.

### Prerequisites

* Functional, deployed application

* GitHub repository with README describing the project

* Navbar must be consistent on each page.

* Navbar on each page must contain links to Home/About, Contact, and Portfolio pages.

* All links must work.

* Must use semantic html.

* Each page must have valid and correct HTML. (use a validation service)

* Must contain your personalized information. (bio, name, images, links to social media, etc.)

* Must properly utilize Bootstrap components and grid system.


### Break down
  ## Copy & Paste + Changes
I wanted to focus on making sure that the header, navigation and footer were all universal in each page and respond the same. To ensure that, I foused on working on the index.html page first then copy and pasted those tags into the rest of the contact.html & portfolio.html pages. I changed the active navs to ensure that it is accurate and to let the user know which page they are on. I also changed the h2 tags to ensure the title of those pages are accurate as well. 
  
```html
<h2>About Me</h2> <h2>Portfolio</h2> <h2>Contact</h2>
```

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About</title>
    <!--Font-->
    <link href="https://fonts.googleapis.com/css2?family=Yanone+Kaffeesatz:wght@200;300;400;500;600;700&display=swap"
        rel="stylesheet">
    <!--CSS-->
    <link rel="stylesheet" href="css/reset.css">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css"
        integrity="sha384-9aIt2nRpC12Uk9gS9baDl411NQApFmC26EwAOH8WgZl5MYYxFfc+NcPb1dKGj7Sk" crossorigin="anonymous">
    <link rel="stylesheet" href="css/style.css">
</head>
```

```html
<header>
        <!--This is the Navigation-->
        <nav class="navbar navbar-light bg-light">

            <!--Header H1-->
            <div class="alert alert-primary" role="alert">
                <h1 class="alert-heading">Marc Anthony Surio</h1>
            </div>

            <!--ul navigation-->
            <ul class="nav nav-pills justify-content-end">
                <li class="nav-item">
                    <a class="nav-link active" href="index.html">About</a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="portfolio.html">Portfolio</a>
                </li>

                <li class="nav-item">
                    <a class="nav-link" href="contact.html">Contact</a>
                </li>
            </ul>
        </nav>
    </header>
```

```html
    <br>
    <!--footer copy and paste-->
    <footer class>
        <div>
            <span>&copy; Copyright of Marc Anthony Surio</span>
        </div>
    </footer>
```

These were the main things that were copied and pasted on each of the pages: index.html, portfolio.html, & contact.html.
The main content were all different but all followed the same format of having a container-fluid, .row, .col-lg, .col-md, .col-sm, and sections.

### And coding style tests

The coding styles for the header and footer and using bootstrap were fairly easy. I felt like that once you had all those components together then you already finished half of the work that you have to do. Bootstrap already uses a template that are very media-query friendly, but you still have to stylize the media queries to make it appealing. Google Chrome inspector is a huge asset and a life saver for this project as I can just inspect an element and then stylize it. 
```css
/*media queries */

/* devices with the pixel sizes of 769px to 980px*/
@media screen and (max-width:980px) and (min-width:769px){
    .container-fluid{
        position:relative;
        width:90%;
        top:0;
    }
}

/*devices with the pixel sizes between 641px and 768px*/
@media screen and (max-width:768px) and (min-width:641px){
    .container-fluid{
        position:relative;
        top:0;
        width:75%;
    }
}

/*devices with a a pixel of 640px and lower*/
@media screen and (max-width: 640px){
    div.alert.alert-primary{
        width:100%;
        text-align:center;
    }

    h1.alert-heading{
        font-size:60px;
    }
    ul.nav.nav-pills.justify-content-end{
        width:100%;
        font-size:24px;
    }
    
    li.nav-item{
        margin-right:15%;
    }

    h2{
        width:100%;
        text-align:center;
        font-size:54px;
    }

    div.col-lg-4.col-md-4.col-sm-4{
        max-width:100%;
        flex-basis:100%;
    }

    section.col-lg-8.col-md-7.col-sm-7{
        max-width:100%;
        flex-basis: 100%;
        padding:10px;
    }

}
```

## Deployment

https://msurio.github.io/responsive-portfolio/

## Built With

* Visual Studio Code (Ver 1.47)
* Install bootstrap -v 4.5.0

