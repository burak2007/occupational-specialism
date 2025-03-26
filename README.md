phpmyadmin. 
Right click anywhere, go tools, quick add then phpmyadmin.
start server and type in localhost/phpmyadmin = clicking database

LOGIN = root. no password

click new, create database, put name.

no caps or spaces in database.

screenshot my drawsql diagram, ask chatgpt to make it into SQL code phpmyadmin and for MySQL. press go, go on structure tab, and press data dictionary and take screenshots of the tables.

create a table, And then you can see the overview if you click on data dictionary 

when using the code for the website, unzip the folder first then open folder on vscode

video for tryout code
https://youtu.be/oYRda7UtuhA?si=a8mM2ZRBVttBLLpM


<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content=""with=device-width, initial-scale="1.0">
        <title>Rolsa Technologies</title>
        <link rel="stylesheet" href="style.css">
        <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Dosis:wght@200..800&family=Lexend+Deca:wght@100..900&display=swap" rel="stylesheet">
    </head>
    <body>
        <section class="header">
            <nav>
                <a href="index.html"><img src="img/logo.png"></a>
                <div class="nav-links">
                    <ul>
                        <li><a href="">HOME</a></li>
                        <li><a href="">ABOUT</a></li>
                        <li><a href="">SERVICES</a></li>
                        <li><a href="">PROJECTS</a></li>
                        <li><a href="">CONTACT</a></li>
                    </ul>
                </div>
            </nav>

        <div class="text-box">
            <h1>The Path to a Greener Society</h1>
            <p>Rolsa Technologies makes clean energy simple with solar panels, EV charging stations, and smart home energy systems.<br> Helping you save money while protecting the planet.</p>
             <a href="" class="hero-btn">Learn More About Us!</a>       
        </div>

        </section>
    </body>

</html>


css

*{
    margin: 0;
    padding: 0;
    font-family: "Lexend Deca", sans-serif;
}
.header{
    min-height: 100vh;
    width: 100%;
    background-image: linear-gradient(rgba(4,9,30,0.7),rgba(4,9,30,0.7)),url(img/bannerpic.png);
    background-position: center;
    background-size: cover;
    position: relative;
}
nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
nav img{
    width: 250px;
}
.nav-links{
    flex: 1;
    text-align: right;
    padding: 8px 50px;
}
.nav-links ul li{
    list-style: none;
    display: inline-block;
    padding: 8px 12px;
    position: relative;
}
.nav-links ul li a{
    color: #fff;
    text-decoration: none;
    font-size: 20px;
}
.nav-links ul li::after{
    content: '';
    width: 0%;
    height: 2px;
    background: #2ab425;
    display: block;
    margin: auto;
    transition: 0.5s;
}
.nav-links ul li:hover::after{
    width: 100%; 
}
.text-box{
    width: 90%;
    color: #fff;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    text-align: center;
}
.text-box h1{
    font-size: 62px;
}
.text-box p{
    margin: 10px 0 40px;
    font-size: 16px;
    color: #fff;
}
.hero-btn{
    display: inline-block;
    text-decoration: none;
    color: #fff;
    border: 1px solid #fff;
    padding: 12px 34px;
    font-size: 13px;
    background: transparent;
    position: relative;
    cursor: pointer;
}
.hero-btn:hover{
    border: 1px solid #1fad26;
    background: #1fad26;
    transition: 1s;
}

nav .fa{
    display: none;
}

@media(max-width: 700px){
    .text-box h1{
        font-size: 20px;
    }
    .nav-links ul li{
        display: block;
    }
    .nav-links{
        position: absolute;
        background: #1fad26;
        height: 100vh;
        width: 200px;
        top: 0;
        right: 0;
        text-align: left;
        z-index: 2;

    }
    nav .fa{
        display: block;
        color: #fff;
        margin: 10px;
        font-size: 22px;
        cursor: pointer;
    }
    .nav-links ul{
        padding: 30px;
        
    }
}
