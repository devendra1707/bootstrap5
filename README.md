# bootstrap5qaj5gyi

Bootstrap 5
- HTML - DOM
- CSS - Sass or Less
- Bootstrap

                                        Bootstrap
- It is an open source and cross platform library for building effective, responsive UI faster.
- Library provides
        a) Utilities
        b) Components
- Utilities are used for changing the appearence of any element
        font, style, color, position, display, margin, padding etc..
- Components are rich in UI, styles and Logic.
        Cars, Buttons, Forms, Accordion, Alerts, Modals, Navbar etc...

Alternatives:
            TwitterBootstrap
            mui [Material UI]    - React [Netflix, Facebook, Amazon]
            Material UI            - Angular
            Telerik                - JSP, PHP, React, Angular, ASP.NET
            DevExpress        
            jQueryUI


                                      Setup Project
1. Download and Install
            "Visual Studio Code Editor"
   
2. Create a folder for project on your PC

             D:\Bootstrap-workshop

3. Open folder in Visual Studio Code

4. Add folders
            public                : It is for static resources like : html, image, docs
            src                    : It is for dynamic resources like: css, js, sass, ts etc..

5. Add a startup page "Index.html"  in public folder

6. Test your page by opening with Live Server
   
     [Visual Studio Code - Extentions - Download Live Server Extention]


7. Right Click in HTML page => Open with Live Server | Open In Browser

                       
                            Enable Bootstrap Icons for your Page
                            ---------------------------------------------------

1. Visit the website
            www.getbootstrap.com

2. Go to "Icons" category and copy its CSS  CDN link and paste in your page
        <head>

Syntax:
    <head>
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    </head>

    - Bootstrap ICONS are provided as CSS classes, which you can implement
      in page.

                <span  class="bi bi-house">
                <span  class="bi bi-bell">
                <span  class="bi bi-facebook">

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
</head>
<body>
    <h1> <span class="bi bi-basket-fill"></span> Shopping Online</h1>
    <p>Follow us on <span class="bi bi-facebook"></span> Facebook <span class="bi bi-twitter"></span> Twitter  <span class="bi bi-instagram"></span> Instagram</p>
</body>
</html>

                        Enable Bootstrap Utilities and Components

1. Visit "www.getbootstrap.com&quot;

2. Click on Download

3. Copy CDN links for CSS and jQuery

                bootstrap.css
                bootstrap.bundle.js
                poper.js [2 components  dropdown positions, tooltip]

    Paste    CSS Link  in  <head>
    Paste  Script Link in <body>


Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body>

    <h1> <span class="bi bi-basket-fill"></span> Shopping Online</h1>
    <p>Follow us on <span class="bi bi-facebook"></span> Facebook <span class="bi bi-twitter"></span> Twitter  <span class="bi bi-instagram"></span> Instagram</p>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

Summary
- bootstrap-icons.css            ]  head
- bootstrap.min.css            ]
- bootstrap.bundle.min.js        ]  body


                                     Layout Classes

.container                        Mobiles  540px
.container-sm                    Tab
.container-lg                        PC [1200px]
.container-md                    PC [1300px]
.container-xl                        Laptop [1400px]
.container-xxl                    Laptop [1600px]
.container-fluid                    Responsive

                                    Box Model Classes
                                    ---------------------------
- Box model comprises of
        1. margin
        2. padding
        3. border
        4. border-radius
        5. width
        6. height

Margins:
        .m                margin all directions
        .ms            margin-left [start]  [ <5 ml ]
        .me            margin-right[end]
        .mt            margin-top
        .mb            margin-bottom
        .mx            margin-x-axis
        .my            margin-y-axis

        Break-Point
        {1 to 4}

Syntax:
            <div class="me-4 ms-3">

Ex:
 <h1 class="ms-4 mt-4"> <span class="bi bi-basket-fill"></span> Shopping Online</h1>
    <p class="ms-4 mt-4">Follow us on <span class="bi bi-facebook me-2"></span> Facebook <span class="bi bi-twitter"></span> Twitter  <span class="bi bi-instagram"></span> Instagram</p>

Padding:
          .p
          .ps
          .pe
          .pt
          .pb
          .px
          .py

    Break-Point : {1 to 4}

Border  :
        .border
        .border-{1 to 3}
        .border-{primary | danger | success | warning | infor | dark }
       
Radius :
        .rounded
        .rounded-{1 to 3}
        .rounded-pill
        .rounded-circle

Width:
        .w- {25, 50, 75, 100}
Height:
        .h- {25, 50, 75, 100}

Text Colors:
 .text-{contextual }

Background Color:
 .bg-{contextual}
 
 Summary
- Adding CDN Links
        bootstrap-icons.css
        bootstrap.css
        bootstrap.bundle.js
- Icons classes
        bi bi-house
- Bootstrap classes
        margins
        padding
        border
        rounded
        width
        height
        text color
        bg color

                                       Display Classes

.d-none                display none
.d-block                display block
.d-inline                display inline
.d-flex                    display flex

Ex: Inline is applied to elements in container

 <nav>
        <div class="d-inline">Home</div>
        <div class="d-inline">About</div>
        <div class="d-inline">Contact</div>
 </nav>

Ex: Flex is applied to container

    <nav class="d-flex">
        <div>Home</div>
        <div>About</div>
        <div>Contact</div>
     </nav>

- Flex can have alignment and direction

    .justify-content-between
    .justify-content-center
    .justify-content-baseline
    .align-items-center
    .align-items-baseline
    .flex-wrap
    .flex-row
    .flex-column

Ex:
  <nav class="d-flex justify-content-between">
        <div>Home</div>
        <div>About</div>
        <div>Contact</div>
        <div>Electronics</div>
        <div>Footwear</div>
  </nav>

FAQ: How to keep any content exaclty center of page?
Ans : d-flex, justify-content-center, align-items-center

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <div class="d-flex justify-content-center align-items-center" style="height:500px">
        <form class="border border-primary p-2 border-3">
            <h2>User Login</h2>
            <dl>
                <dt>User Name</dt>
                <dd><input type="text"></dd>
                <dt>Password</dt>
                <dd><input type="password"></dd>
            </dl>
            <button>Login</button>
        </form>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>


Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body style="height:400px"  class="container-fluid d-flex justify-content-center align-items-center">
    <div class="text-center">
        <h1>Neflix</h1>
        <p>Watch movies, tv shows online.</p>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <header class="d-flex justify-content-between bg-dark text-white p-2">
        <div>Shopper</div>
        <div>
            <span class="me-3">Home</span>
            <span class="me-3">Catalog</span>
            <span class="me-3">Shop</span>
            <span class="me-3">Blog</span>
            <span class="me-3">Pages</span>
        </div>
        <div>
            <span class="bi bi-search me-3"></span>
            <span class="bi bi-person me-3"></span>
            <span class="bi bi-heart me-3"></span>
            <span class="bi bi-cart me-3"></span>
        </div>
    </header>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

                                      Positions
.position-relative
.position-fixed
.position-absolute
.position-static
.position-sticky

.top-{0,25,50,75,100}
.bottom
.start
.end

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid" style="height:500px">
     <h2>Positions</h2>
     <div class="position-fixed end-0 bottom-0">
        <div class="bi bi-facebook"></div>
        <div class="bi bi-twitter"></div>
        <div class="bi bi-instagram"></div>
     </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <h2>Categories</h2>
    <dl>
        <dt class="bg-dark text-white p-2 position-sticky top-0">Electronics</dt>
        <dd>Mobiles</dd>
        <dd>Televisions</dd>
        <dd>Watch</dd>
        <dd>Mobiles</dd>
        <dd>Televisions</dd>
        <dd>Watch</dd>
        <dd>Mobiles</dd>
        <dd>Televisions</dd>
        <dd>Watch</dd>
        <dd>Mobiles</dd>
        <dd>Televisions</dd>
        <dd>Watch</dd>
        <dd>Mobiles</dd>
        <dd>Televisions</dd>
        <dd>Watch</dd>
        <dd>Mobiles</dd>
        <dd>Televisions</dd>
        <dd>Watch</dd>
        <dd>Mobiles</dd>
        <dd>Televisions</dd>
        <dd>Watch</dd>
        <dd>Mobiles</dd>
        <dd>Televisions</dd>
        <dd>Watch</dd>
        <dd>Mobiles</dd>
        <dd>Televisions</dd>
        <dd>Watch</dd>
        <dt class="bg-dark text-white p-2 position-sticky top-0">Footwear</dt>
        <dd>Boots</dd>
        <dd>Casuals</dd>
        <dd>Sneakers</dd>
        <dd>Boots</dd>
        <dd>Casuals</dd>
        <dd>Sneakers</dd>
        <dd>Boots</dd>
        <dd>Casuals</dd>
        <dd>Sneakers</dd>
        <dd>Boots</dd>
        <dd>Casuals</dd>
        <dd>Sneakers</dd>
        <dd>Boots</dd>
        <dd>Casuals</dd>
        <dd>Sneakers</dd>
        <dd>Boots</dd>
        <dd>Casuals</dd>
        <dd>Sneakers</dd>
        <dd>Boots</dd>
        <dd>Casuals</dd>
        <dd>Sneakers</dd>
        <dd>Boots</dd>
        <dd>Casuals</dd>
        <dd>Sneakers</dd>
        <dd>Boots</dd>
        <dd>Casuals</dd>
        <dd>Sneakers</dd>
    </dl>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

                                    Rows and Columns [Grid]
.row
.col
.col-{1 to 12}


Ex:
 <h2>Product Details</h2>
    <dl class="row">
        <dt class="col-2">Name</dt>
        <dd class="col-10">Nike Casuals</dd>
        <dt class="col-2">Price</dt>
        <dd class="col-10">5600.44</dd>
        <dt class="col-2">Stock</dt>
        <dd class="col-10">Available</dd>
    </dl>


Ex:
 <h2>Columns</h2>
     <div class="row">
        <div class="col-2 border border-2 border-primary">Col-1</div>
        <div class="col-8 border border-2 border-primary">Col-2</div>
        <div class="col-2 border border-2 border-primary">Col-3</div>
     </div>
     <div class="row mt-2">
        <div class="col-6 border border-2 border-primary">Col-1</div>
        <div class="col-6 border border-2 border-primary">Col-2</div>
     </div>

Summary
- Display
- Position
- Rows and Columns

                                        Font Styles
.fw-bold                bold
.fst-italic                italic
.fs-{1 to 6}            size

Syntax:
 <p class="mt-3">Welcome to <span class="fw-bold fst-italic fs-5">Bootstrap</span></p>

                                        Text Effects
.text-center
.text-start
.text-end
.text-justify
.text-{contextual}

                                    Bootstrap Components
1. alerts
    - Embedded message boxes in page.
    - You can control with jQuery attributes

classes:
 .alert
 .alert-dismissible
 .alert-{contextual}
 .alert-title
 .alert-subtitle
 .alert-text
 .alert-link

attributes:
 data-bs-dismiss            close any component

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <h2>Alerts</h2>
    <div class="alert alert-danger alert-dismissible">
        <h1 class="alert-title">Delete Record</h1>
        <button class="btn-close" data-bs-dismiss="alert"></button>
        <p class="alert-subtitle">Record will be deleted.</p>
        <a class="alert-link">Help?</a>
    </div>
    <div class="alert alert-success">
        <h1 class="alert-title">Record Inserted</h1>
        <p class="alert-subtitle">Record inserted successfully..</p>
        <button data-bs-dismiss="alert">OK</button>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

2. Buttons

.btn
.btn-{contextual}
.btn-outline-{contextual}
.btn-group
.btn-group-vertical
.btn-link
.btn-close etc..

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
     <h2>Button Contextual</h2>
     <button class="btn btn-danger">Insert</button>
     <button class="btn btn-outline-danger">Insert</button>
     <button class="btn-close"></button>
     <button class="btn btn-link">Logout</button>
     <h2>Button Group</h2>
     <div class="btn-group">
        <button class="btn btn-primary">Prev.</button>
        <button class="btn btn-danger">Next</button>
     </div>
     <h2>Button Group Verical</h2>
     <div class="btn-group-vertical">
        <button class="btn btn-danger mb-2">Home</button>
        <button class="btn btn-danger mb-2">About</button>
        <button class="btn btn-danger mb-2">Contact</button>
     </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

3. Cards

.card
.card-header
.card-body
.card-footer
.card-title
.card-subtitle
.card-img-top
.card-img-overlay

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <main class="d-flex">
        <div class="card p-2 m-2" style="width:250px">
            <img src="ui.jpg" class="card-img-top">
            <div class="card-header text-center">
                <p class="fw-bold text-center">UI Technologies</p>
                <p>Online Training</p>
            </div>
            <div class="card-body text-center text-warning">
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
            </div>
            <div class="card-footer">
                <button class="btn btn-primary w-100">Join Course</button>
            </div>
        </div>
        <div class="card p-2 m-2" style="width:250px">
            <img src="ng.jpg" class="card-img-top">
            <div class="card-header text-center">
                <p class="fw-bold text-center">Angular JS</p>
                <p>Online Training</p>
            </div>
            <div class="card-body text-center text-warning">
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
            </div>
            <div class="card-footer">
                <button class="btn btn-primary w-100">Join Course</button>
            </div>
        </div>
        <div class="card p-2 m-2" style="width:250px">
            <img src="rpa.jpg" class="card-img-top">
            <div class="card-header text-center">
                <p class="fw-bold text-center">RPA</p>
                <p>Online Training</p>
            </div>
            <div class="card-body text-center text-warning">
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
                <span class="bi bi-star-fill"></span>
            </div>
            <div class="card-footer">
                <button class="btn btn-primary w-100">Join Course</button>
            </div>
        </div>
    </main>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

Forms
.form-label                <Label>
.form-control            textbox, password, number, date, email, url etc..
.form-select                <select>
.form-range                <input type="range">
.form-check-input        radio and checkbox
.form-switch                radio and checkbox as switch

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <main class="d-flex justify-content-center align-items-center" style="height:500px" >
        <form class="border border-primary border-1 p-2 rounded rounded-2" style="width:300px">
            <h3>Register User</h3>
            <div class="mb-3">
                <label class="form-label">User Name</label>
                <div>
                    <input type="text" class="form-control">
                </div>
            </div>
            <div class="mb-3">
                <label class="form-label">Password</label>
                <div>
                    <input type="password" class="form-control">
                </div>
            </div>
            <div class="mb-3">
                <label class="form-label">City</label>
                <div>
                    <select class="form-select">
                        <option>Your City</option>
                        <option>Delhi</option>
                        <option>Hyd</option>
                    </select>
                </div>
            </div>
            <div class="mb-3">
                <label class="form-label">Age</label>
                <div>
                    <input type="range" class="form-range">
                </div>
            </div>
            <div class="mb-3">
                <label class="form-label">Subscribe</label>
                <div class="form-switch">
                    <input type="checkbox" class="form-check-input"> <label>Yes</label>
                </div>
            </div>
            <div>
                <button class="btn btn-primary w-100">Register</button>
            </div>
        </form>
    </main>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

                                       Input Group
.input-group
.input-group-text
.input-group-lg

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <h2>Amazon Search</h2>
    <div class="input-group">
        <select class="input-group-text">
            <option>All</option>
            <option>Mobiles</option>
            <option>Fashion</option>
        </select>
        <input type="text" class="form-control" placeholder="Search in Amazon">
        <button class="btn btn-warning">
            <span class="bi bi-search"></span>
        </button>
    </div>
    <h2>Neflix</h2>
    <div class="input-group input-group-lg">
        <input class="form-control" type="email" placeholder="Your email address">
        <button class="btn btn-danger">
            Get Started <span class="bi bi-chevron-right"></span>
        </button>
    </div>
    <h3>Verify Account</h3>
    <div class="input-group">
        <span class="bi bi-key-fill input-group-text"></span>
        <input type="password" class="form-control" placeholder="Your password">
        <button class="btn btn-success">Verify</button>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

                                          Modals
.modal
.modal-dialog
.modal-content
.modal-header
.modal-body
.modal-footer
.fade

data-bs-toggle                : click
data-bs-target                : It refers to ID
data-bs-dismiss

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
     <h2>Dialog - Modal</h2>
     <button class="btn btn-primary" data-bs-target="#login" data-bs-toggle="modal">Login</button>
     <button class="btn btn-success" data-bs-target="#course" data-bs-toggle="modal" >View Course</button>
     <div class="modal fade" id="login">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h2>User Login</h2>
                    <button class="btn-close" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body">
                    <dl>
                        <dt>User Name</dt>
                        <dd><input type="text" class="form-control"></dd>
                        <dt>Password</dt>
                        <dd><input type="password" class="form-control"></dd>
                    </dl>
                </div>
                <div class="modal-footer">
                    <button class="btn btn-primary">Login</button>
                    <button data-bs-dismiss="modal" class="btn btn-danger">Cancel</button>
                </div>
            </div>
        </div>
     </div>

     <div class="modal fade" id="course">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h2>UI Technologies</h2>
                    <button class="btn-close" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body">
                    <div class="row">
                        <div class="col-4">
                            <img src="ui.jpg" width="100" height="100">
                        </div>
                        <div class="col-8">
                            <ol>
                                <li>HTML</li>
                                <li>CSS</li>
                                <li>Bootstrap</li>
                                <li>JavaScript</li>
                            </ol>
                        </div>
                    </div>
                </div>
            </div>
        </div>
     </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

                                         Carousel
Basic Classes
.carousel
.carousel-inner
.carousel-item
.active                    : One Item must be active
.slide                        : It defines sliding animation

Attribute
data-bs-ride            : to start animation

Control Classes
.carousel-control-prev
.carousel-control-prev-icon
.carousel-control-next
.carousel-control-next-icon
.carousel-dark

Attribute
data-bs-slide="prev"
data-bs-slide="next"
data-bs-target="#bannerId"

Indicator Classes
.carousel-indicators
.active

Attribute
data-bs-slide-to="0"

Timings
data-bs-interval="1000"        // 1 sec

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <div class="carousel slide carousel-dark" id="topBanner" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active" data-bs-interval="3000">
                <img src="slide1.jpg" class="w-100 d-block">
            </div>
            <div class="carousel-item" data-bs-interval="1000">
                <img src="slide2.jpg" class="w-100 d-block">
            </div>
            <div class="carousel-item" data-bs-interval="5000">
                <img src="slide3.jpg" class="w-100 d-block">
            </div>
        </div>
        <button class="carousel-control-prev" data-bs-target="#topBanner" data-bs-slide="prev">
            <span class="carousel-control-prev-icon"></span>
        </button>
        <button class="carousel-control-next" data-bs-target="#topBanner" data-bs-slide="next">
            <span class="carousel-control-next-icon"></span>
        </button>
        <div class="carousel-indicators">
            <button class="active" data-bs-slide-to="0" data-bs-target="#topBanner"></button>
            <button data-bs-slide-to="1" data-bs-target="#topBanner"></button>
            <button data-bs-slide-to="2" data-bs-target="#topBanner"></button>
        </div>
    </div>  
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>


Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <div class="carousel slide carousel-dark" id="topBanner" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active" data-bs-interval="3000">
                <img src="slide1.jpg" class="w-100 d-block">
            </div>
            <div class="carousel-item" data-bs-interval="1000">
                <img src="slide2.jpg" class="w-100 d-block">
            </div>
            <div class="carousel-item" data-bs-interval="5000">
                <div class="d-flex justify-content-center align-items-center" style="height:250px">
                    <div>
                        <h1>Register with us for more offers</h1>
                        <button class="btn btn-primary btn-lg">Register</button>    
                    </div>
                </div>
            </div>
            <div class="carousel-item" data-bs-interval="5000">
                <img src="slide3.jpg" class="w-100 d-block">
            </div>
        </div>
        <button class="carousel-control-prev" data-bs-target="#topBanner" data-bs-slide="prev">
            <span class="carousel-control-prev-icon"></span>
        </button>
        <button class="carousel-control-next" data-bs-target="#topBanner" data-bs-slide="next">
            <span class="carousel-control-next-icon"></span>
        </button>
        <div class="carousel-indicators">
            <button class="active" data-bs-slide-to="0" data-bs-target="#topBanner"></button>
            <button data-bs-slide-to="1" data-bs-target="#topBanner"></button>
            <button data-bs-slide-to="2" data-bs-target="#topBanner"></button>
            <button data-bs-slide-to="3" data-bs-target="#topBanner"></button>
        </div>
    </div>  
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>

                                        Dropdowns
.dropdown
.dropup
.dropend
.dropstart
.dropdown-menu
.dropdown-item
.dropdown-toggle

Ex:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <h2>Dropdown</h2>
    <div class="dropdown" id="menu">
        <button class="btn btn-dark dropdown-toggle" data-bs-toggle="dropdown">
            <span class="bi bi-globe"></span> Language
        </button>
        <ul class="dropdown-menu dropdown-menu-dark">
            <li class="dropdown-item">English</li>
            <li class="dropdown-item">हिंदी</li>
        </ul>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>
                                            Spinners
.spinner-grow

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap-Workshop</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css"&gt;
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css&quot; rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>
<body class="container-fluid">
    <h2>Dropdown</h2>
    <div class="dropdown" id="menu">
        <button class="btn btn-dark dropdown-toggle" data-bs-toggle="dropdown">
            <span class="spinner-border spinner-border-sm text-warning"></span> Language
        </button>
        <ul class="dropdown-menu dropdown-menu-dark">
            <li class="dropdown-item">English</li>
            <li class="dropdown-item">हिंदी</li>
        </ul>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js&quot; integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>
