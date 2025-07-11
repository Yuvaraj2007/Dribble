# Project Responsive Web Design using Bootstrap
## Date:

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8" />
    <meta name="viewport" 
          content="width=device-width, 
                   initial-scale=1" />

    <!-- Bootstrap CSS -->
    <link
      href=
"https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta2/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity=
"sha384-BmbxuPwQa2lc/FVzBcNJ7UAyJxM6wuqIj61tLrc4wSX0szH/Ev+nYRRuWlolflfl"
      crossorigin="anonymous"
    />
    <link rel="stylesheet"
          href="style.css" />
    <link rel="preconnect" 
          href="https://fonts.gstatic.com" />
    <link
      href=
"https://fonts.googleapis.com/css2?family=Roboto+Condensed&display=swap"
      rel="stylesheet"
    />
    <title>Project</title>
  </head>
  <body>
    <style>
        *{
    margin: 0;
    padding: 0;
    font-family: 'Roboto Condensed', sans-serif;
}

/* navbar */

.navbar-nav{
    margin-right: 0 !important;
    padding-right: 100px;
}

.navbar{
    background-color: #0a193d;
    color: white !important;
}

.nav-item a{
    color: white !important;
}

.nav-item{
    padding-left: 2px;
}

.navbar-brand{
    color: white !important;
    padding-left: 100px;
}

#navbar button{
    color: white !important;
}

/* banner */

#banner-container{
    background-color: #0a193d;
    color: white !important;
    padding-top: 80px;
    padding-bottom: 80px;
    
}

#banner-row img{
    max-width: 70%;
    height: auto;
    display: block;
    padding-left: 30px;
}

#banner-row h3, p{
    padding-left: 20px;
    padding-top: 20px;
    text-align: center;
}

#banner-row a{
    background-color: white !important;
    color: black !important;
    border: none;
    margin-left: 20px;
    margin-top: 20px;
    
}
#banner-col{
    padding-left: 20px;
}
/* service */
#service{
    padding-top: 80px;
    padding-bottom: 80px;
}

#service h1{
    padding-bottom: 70px;
}
    </style>
    <section id="navbar">
      <nav class="navbar navbar-expand-lg navbar-light">
        <div class="container-fluid">
          <a class="navbar-brand" href="#">
              Dribble
            </a>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" 
               id="navbarSupportedContent">
            <ul class="navbar-nav m-auto">
              <li class="nav-item">
                <a class="nav-link active" 
                   aria-current="page" 
                   href="#">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" 
                   href="#service">Services</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" 
                   href="#social">Contact Us</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </section>

    <!-- banner -->
    <section id="banner">
      <div class="container-fluid" id="banner-container">
        <div class="row" id="banner-row">
          <div class="col-md-6" id="banner-col">
            <h3>
              BEST PROFESSIONAL WEBSITE DESIGN 
              SOFTWARE DEVELOPMENT COMPANY
            </h3>
            
<p>
              The fastest way to grow your business with the leader in
              Technology
            </p>

            <div class="d-grid gap-2 d-md-flex justify-content-center">
              <a class="btn btn-primary" 
                 href="#" 
                 role="button">Contact Us</a>
            </div>
          </div>
          <div class="col-md-6" id="banner-col2">
            <img
              class="img-responsive rounded mx-auto d-block"
              src="images/gfg.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>

    <!-- services -->
    <section id="service">
      <h1 class="text-center">SERVICES</h1>
      <div class="container-fluid" id="service-container">
        <div class="row" id="banner-row">
          <div class="col-md-4" id="service-col1">
            <img
              src="web design.jpg"
              class="img-fluid rounded mx-auto d-block"
              alt="..."
            />
            <h3>Website Design</h3>
            
<p>
              User Experience Design. 
              Website Content Strategy. 
              Cross Browser
              and Platform Testing.
            </p>

          </div>
          <div class="col-md-4" id="service-col2">
            <img
              src="sms.jpg"
              class="img-fluid rounded mx-auto d-block"
              alt="..."
            />
            <h3>Bulk SMS</h3>
            
<p>
              1.Toll Free Number <br>
              2. IVR <br>
              3. Virtual Number <br>
              4. Political or any<br>
              Voice Broadcasting<br>
            </p>

          </div>
          <div class="col-md-4" id="service-col3">
            <img
              src="payment.jpg"
              class="img-fluid rounded mx-auto d-block"
              alt="..."
            />
            <h3>Payment Gateways</h3>
            
<p>
              PayU India is the flagship company of
               Naspers group which is a $25
              Billion internet and media conglomerate
               listed on London and
              Johannesburg stock exchanges respectively.
            </p>

          </div>
        </div>
      </div>
    </section>
    <hr />
    <!-- social -->
    <section id="social">
      <h1 class="text-center">Get In Touch</h1>
      <div class="d-grid gap-2 d-md-flex justify-content-center">
        <div class="row align-items-center" id="social-row">
          <div class="col-md-4 social-col">
            <a href=""
              ><img
                class="img-responsive rounded mx-auto d-block"
                src="images/gfg.png"
                alt=""
            /></a>
          </div>
          <div class="col-md-4 social-col">
            <a href=""
              ><img
                class="img-responsive rounded mx-auto d-block"
                src="images/icons8-instagram-64.png"
                alt=""
            /></a>
          </div>
          <div class="col-md-4 social-col">
            <a href=""
              ><img
                class="img-responsive rounded mx-auto d-block"
                src="images/icons8-twitter-64.png"
                alt=""
            /></a>
          </div>
        </div>
      </div>
    </section>

    <!-- footer -->
    <section id="footer">
      <section id="banner">
        <div class="container-fluid" id="banner-container">
          <div class="row" id="banner-row">
            <div class="col-md-4" id="footer-col1">
              <h3>My Website</h3>
              
<p>
                support@xyz.com
              </p>

            </div>
            <div class="col-md-4" id="footer-col2">
              <h3>Contact Us</h3>
              
<p>Call Us- 1800-121-6532</p>

              
<p>Email Us- support@xyz.com</p>

            </div>

            <div class="col-md-4" id="footer-col2">
              <h3>Subscribe To Newsletter</h3>
              <form>
                <div class="mb-3">
                  <input
                    type="email"
                    placeholder="Enter Your Email"
                    class="form-control"
                    id="exampleInputEmail1"
                    aria-describedby="emailHelp"
                  />
                  <div id="emailHelp" 
                       class="form-text">
                    We'll never share your email with anyone else.
                  </div>
                </div>
                <button type="submit" 
                        class="btn btn-primary">
                        Submit
                </button>
              </form>
            </div>
          </div>
        </div>
      </section>
    </section>

    
    </body>
    </html>
```

## OUTPUT:

![alt text](<Screenshot 2025-05-21 142218.png>)

![alt text](<Screenshot 2025-05-21 142315.png>)


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
