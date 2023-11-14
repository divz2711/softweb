# Ex.07 Software Product Company Website
## Date: 19.10.2023		

## AIM:
To develop a static company website to display the softwares and services provided by the company.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
main.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <link rel="icon" href="Softserves.png">
    <title>Software Development Company</title>
</head>

<body>

    <header>
        <div class="container">
            <h1>SoftServe Innovations</h1>
            <nav>
                <ul>
                    <li><a href="#home">HOME</a></li>
                    <li><a href="#services">SERVICES</a></li>
                    <li><a href="#partners">PARTNERS</a></li>
                    <li><a href="#contact">CONTACT</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="hero">
        <div class="container">
            <h1>Welcome to Softserves</h1>
            <p>Your Gateway to Innovation</p>
            <a href="#contact" class="btn">Get Started</a>
        </div>
    </section>

    <section id="home">
        <div class="container">
            <h2>ABOUT US</h2>
            <p>We are a dynamic team specializing in designing, developing, and maintaining cutting-edge applications,
                frameworks, and software components for businesses. Our passion lies in staying ahead of industry trends,
                adopting the latest technologies, and pioneering innovative solutions.</p>
        </div>
    </section>

    <section id="services">
        <div class="container">
            <h2>SERVICES</h2>
            <div class="service">
                
                <h3>Web Application Development</h3>
                <p>Crafting Solutions with Precision</p>
            </div>
            <div class="service">
                
                <h3>Mobile Application Development</h3>
                <p>Seamless Mobility, Exceptional Experiences</p>
            </div>
            <div class="service">
                
                <h3>Blockchain Development</h3>
                <p>Building Trust through Advanced Security</p>
            </div>
        </div>
    </section>

    <section id="partners">
        <div class="container">
            <h2>OUR PARTNERS</h2>
            <ul class="partner-logos">
                <li>TechSynergy Solutions</li>
                <li>InnovateTech Collaborative</li>
                <li>CodeCraft Alliance</li>
            </ul>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>CONTACT US</h2>
            
            <p>Have questions or compliments? We welcome all. Reach out to us below:</p>
            <form>
                <input type="text" placeholder="Your Name">
                <input type="email" placeholder="Your Email">
                <textarea placeholder="Your Message"></textarea>
                <button type="submit" class="btn">Send</button>
            </form>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2023 DS. All rights reserved.</p>
        </div>
    </footer>

</body>

</html>

styles.css

body, h1, h2, h3, p {
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, sans-serif;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

header {
    background-color: #333;
    color: #fff;
    padding: 10px 0;
}

header img {
    width: 100px;
    height: auto;
}

header h1 {
    display: inline;
    margin-left: 10px;
}

nav ul {
    list-style: none;
    display: inline;
}

nav ul li {
    display: inline;
    margin-left: 20px;
}

nav ul li a {
    text-decoration: none;
    color: #fff;
}

#hero {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 50px 0;
}

#hero h1 {
    font-size: 36px;
    margin-bottom: 20px;
    color: #ffcc00; /* Yellow */
}

#hero p {
    font-size: 18px;
    margin-bottom: 30px;
}

.btn {
    background-color: #fff;
    color: #333;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
    transition: background-color 0.3s ease; /* Smooth transition effect */
}

.btn:hover {
    background-color: #ddd;
}

#home {
    background-color: #eee;
    padding: 50px 0;
}

#home h2 {
    text-align: center;
    font-size: 36px;
    margin-bottom: 20px;
    color: #009688; /* Teal */
}

#home p {
    text-align: center;
    max-width: 800px;
    margin: 0 auto;
}

#services {
    background-color: #fff;
    padding: 50px 0;
}

#services h2 {
    text-align: center;
    font-size: 36px;
    margin-bottom: 20px;
    color: #673ab7; /* Deep Purple */
}

.service {
    text-align: center;
    margin-bottom: 40px;
}

.service img {
    width: 100%;
    max-width: 400px;
    height: auto;
    margin-bottom: 10px;
}

#partners {
    background-color: #eee;
    padding: 50px 0;
}

#partners h2 {
    text-align: center;
    font-size: 36px;
    margin-bottom: 20px;
    color: #ff9800; /* Orange */
}

.partner-logos {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}

.partner-logos img {
    width: 150px;
    height: auto;
    margin-bottom: 20px;
}

#contact {
    background-color: #fff;
    padding: 50px 0;
}

#contact h2 {
    text-align: center;
    font-size: 36px;
    margin-bottom: 20px;
    color: #e91e63; /* Pink */
}

#contact p {
    text-align: center;
    max-width: 800px;
    margin: 0 auto;
}

form {
    max-width: 600px;
    margin: 0 auto;
}

form input,
form textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    box-sizing: border-box;
}

footer {
    background-color: #333;
    color: #fff;
    padding: 20px 0;
    text-align: center;
}

.social-icons a {
    margin-right: 10px;
}

.phone-icon {
    display: inline-block;
    margin-left: 10px;
    cursor: pointer;
}

.hide {
    display: none;
}


```

## OUTPUT:
![image](https://github.com/divz2711/softweb/assets/121245222/df0d2c10-5a84-4fcb-8f7e-18811e29d317)
![image](https://github.com/divz2711/softweb/assets/121245222/5ac6aa0b-2566-4819-a7dc-13f035d8e661)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
