<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cedarville+Cursive&family=Dancing+Script&display=swap"
        rel="stylesheet">
    <style>
        body {
            margin: 0%;
            padding: 0%;
        }

        .header {
            display: grid;
            margin: 0px;
            grid-template-columns: 0.5fr 7fr 1fr;
            background-color: rgb(21, 76, 121);
            grid-column-gap: 320px;
            height: 50px;
        }

        .left {
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .search {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 5px;

        }

        .contactus {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 7px;
        }

        #hlogo {
            height: 40px;
            width: 73px;
        }

        #hsl {
            width: 30px;
            height: 30px;

            background-color: white;
        }

        #hs {
            box-sizing: border-box;
            width: 316px;
            height: 30px;
            border-radius: 10px;
            padding: 15px;

        }

        #contactus button {
            border-radius: 10px;
        }

        .nav {
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0px;
            height: 35px;
            background-color: blue;
        }

        .nav li {
            display: inline-block;
            padding-inline: 25px;
        }

        .nav a {
            text-decoration: none;
            color: white;
        }

        .nav li a:hover,
        .nav li a.active {
            color: yellow;
            text-decoration: underline;
            font-weight: bold;
            font-size: larger;

        }

        ul {
            list-style: none;
            margin: 0px;
        }

        .main {
            display: grid;
            grid-template-columns: 1fr 1fr;
            perspective: 2000px;
        }

        .mainleft {
            display: flex;
            justify-content: center;
            align-items: center;
            background-image: url(/him.jpg);
            background-size: cover;
            height: 100vh;
            font-size: 200px;
            font-family: cursive;
            color: rgb(85, 100, 218);
        }

        .mainright {
            display: flex;
            justify-content: center;
            align-items: center;
            background-image: url(/her.jpg);
            background-size: cover;
            height: 100vh;
            font-size: 200px;
            font-family: cursive;
            color: rgb(225, 113, 132);
        }

        .mainleft:hover {
            transform: rotateY(45deg);
        }

        .mainright:hover {
            transform: rotateY(-45deg);
        }

        .men {
            opacity: 0;
            background-color: rgb(152, 152, 215);
            position: absolute;
            left: 445px;
            top: 250px;
            display: inline-block;
            color: black;
            transform: rotateY(45deg);
            font-size: large;

        }

        .women {
            opacity: 0;
            background-color: pink;
            position: absolute;
            left: 757px;
            top: 380px;
            display: inline-block;
            color: black;
            transform: rotateY(-45deg);
            font-size: large;
        }

        .mainleft:hover .men {
            opacity: 1;
        }

        .mainright:hover .women {
            opacity: 1;
            transform: translateX(-850px);
        }
    </style>
</head>

<body>
    <div class="header">
        <div class="left">
            <img src="./logo.png" id="hlogo">

        </div>
        <div class="search">
            <input type="text" id="hs" placeholder="Search here">
            <img src="/icons8-search-100.png" id="hsl">

        </div>
        <div class="contactus">
            <a href="/contactus.html"><button type="button" class="hsl" id="contactus button">Contact us</button></a>
        </div>
    </div>
    <div class="nav">
        <ul>
            <li><a href="/Home.html" class="active">Home</a></li>
            <li><a href="/offers.html">Offers</a></li>
            <li><a href="/sellers.html">About Sellers</a></li>
            <li><a href="about us.html">About the Site and our Aim</a></li>
        </ul>
    </div>
    <div class="main">
        <div class="mainleft"> For him
            <div class="men">
                <ul>
                    <li><a href="/t-shirts.html">T-shirts</a></li>
                    <li><a href="/button down shirt.html">Button-down shirts</a></li>
                    <li><a href="/shoes.html">Shoes (Sneakers, Dress Shoes, Boots, etc.)</a></li>
                </ul>
            </div>
        </div>
        <div class="mainright">For her
            <div class="women">
                <ul>
                    <li><a href="/dresses.html">Dresses</a></li>
                    <li><a href="/tops.html">Tops</a></li>
                    <li><a href="/pants.html">Pants</a></li>
                </ul>
            </div>
        </div>
    </div>


</body>

</html>
