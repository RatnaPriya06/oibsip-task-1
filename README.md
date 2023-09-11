HTML

<!DOCTYPE html>
<html lang="en">
  
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content=
        "width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="index.css">
    <title>Landing Page</title>
</head>
  
<body>
    <nav>
        <div class="heading">Landing Page</div>
        <span class="sideMenuButton" 
            onclick="openNavbar()">
            ☰
        </span>
  
        <div class="navbar">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Sign Up</a></li>
            </ul>
        </div>
    </nav>
  
    <!-- Side navigation bar for 
        responsive website -->
    <div class="sideNavigationBar" 
        id="sideNavigationBar">
        <a href="#" class="closeButton" 
            onclick="closeNavbar()">
            ❌
        </a>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Sign Up</a>
    </div>
  
    <!-- Content -->
    <div class="line" id="Home">
        <div class="side1">
            <h1>VPN</h1>
            <h4>Most trusted free VPN</h4>
            <button>
                <a href=
"https://chrome.google.com/webstore/detail/free-vpn-for-chrome-vpn-p/majdfhpaihoncoakbjgbdhglocklcgno">
                    Get Free VPN
                </a>
            </button>
        </div>
        <div class="side2">
            <img src=
"C:\Users\Ratna Priya\OneDrive\Desktop\R\R2\Images\vpn.png"
                width="500">
        </div>
    </div>
  
    <section class="about" id="My Projects">
        <div class="content">
            <div class="title">
                <span>Courses</span>
            </div>
            <div class="boxes">
                <div class="box">
                    <div class="topic">
                        <a href="" target="_blank">
                            <u>Turbo VPN</u>
                        </a>
                    </div>
                    <p>
                        Turbo VPN Extension for Chrome browser provides 
                        you with free and unlimited access to all blocked
                        websites and network protection for online activities. 
                        Go online freely with no time limit and interruption.
                    </p>
                </div>
                <div class="box">
  
                    <div class="topic">
                        <a href="" target="_blank">
                            <u>Secure VNP</u>
                        </a>
                    </div>
                    <p>
                        Secure VPN encrypts your Internet connection 
                        so that third parties can’t track your online activity, 
                        making it more secure than a typical proxy, 
                        make your Internet's safety and security, 
                        especially when you using public free Wi-Fi.
                    </p>
                </div>
  
                <div class="box">
                    <div class="topic">
                        <a href="" target="_blank">
                            <u>Thunder VNP</u>
                        </a>
                    </div>
                    <p>
                        Thunder VPN is a very fast application and offers free 
                        VPN proxy service. No settings required, just click a button, 
                        you can access the Internet securely and anonymously.
                    </p>
                </div>
            </div>
        </div>
    </section>
  
    <section class="contact" id="contact">
        <div class="content">
            <div class="title"><span>Sign Up</span></div>
            <div class="contactMenu">
                <div class="input1">
                    <div class="label1">Your Name</div>
                    <div class="input2">
                        <input type="text" 
                            placeholder="Enter your Name here">
                    </div>
                    <div class="label1">
                        <label>Your Email</label>
                    </div>
                    <div class="input2">
                        <input type="text" 
                            placeholder="Enter your Email here">
                    </div>
                    <div class="label1">
                        <label>Your Password</label>
                    </div>
                    <div class="input2">
                        <input type="text" 
                            placeholder="Enter your Password here">
                    </div>
                    <div class="button">
                        <button>Sign Up</button>
                    </div>
                </div>
                <div class="input3">
                    <div class="rightside1">
                        <div class="title1">
                            <span>
                                Contact Us
                            </span>
                        </div>
                        <div class="content1">
                            S 95, First Floor, Greater Kailash-1, 
                            A Block, GK 2, Greater Kailash, 
                            New Delhi, Delhi 110048
                        </div>
                        <div class="title1">
                            <span>More Information</span>
                        </div>
                        <div class="content1">
                            Greetings to all out there!
                            We welcome you to the platform where we
                            consistently strive to offer the best 
                            of networks. This platform has been 
                            designed or all the people who stay outside 
                            and has to use their local network.
                            We have number of free downloads,
                            which makes easily to use any in the world.
                            Thank you for choosing and supporting us!
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Footer section -->
    <footer>
        <div class="footer">
            <span>
                Created By
                <a href="https://openvpn.net/" 
                    target="_blank">
                    OpenVPN
                </a>
            </span>
        </div>
    </footer>
    <script src="index.js"></script>
</body>
  
</html>

CSS 

* {
	padding: 0;
	margin: 0;
	box-sizing: border-box;
}

body {
	background-color: black;
	color: white;
	font-family: "Fira Sans", sans-serif;
	background-color: black;
}

nav {
	width: 100%;
	height: 80px;
	display: flex;
	justify-content: space-between;
	padding: 20px 5%;
	background-color: #447a88;
}

nav .heading {
	font-size: 30px;
	font-weight: 700;
	color: white;
}

nav ul {
	display: flex;
	list-style: none;
}

nav ul li {
	padding: 8px 15px;
	border-radius: 10px;
	transition: 0.2s ease-in;
}

nav ul li a {
	color: black;
	font-size: 20px;
	font-weight: 500;
	text-decoration: none;
	color: white;
}

nav ul li:hover {
	background-color: green;
}

nav ul li a:hover {
	color: white;
}

nav .sideMenuButton {
	font-size: 30px;
	font-weight: bolder;
	cursor: pointer;
	display: none;
}

/* responsive navbar css */
@media screen and (max-width: 600px) {
	nav .sideMenuButton {
		display: flex;
	}

	nav .navbar {
		display: none;
	}

	.sideNavigationBar {
		display: block !important;
	}
}

.sideNavigationBar {
	height: 100%;
	position: fixed;
	top: 0;
	right: 0%;
	background-color: green;
	overflow-x: hidden;
	transition: 0.3s ease-in;
	padding-top: 60px;
	display: none;
}

.sideNavigationBar a {
	padding: 8px 8px 8px 40px;
	display: block;
	font-size: 25px;
	font-weight: 500;
	color: #8d8d8d;
	transition: 0.3s;
	text-decoration: none;
}

.sideNavigationBar a button {
	padding: 10px 20px;
	border-radius: 10px;
	color: green;
	font-size: 16px;
	border-style: none;
	font-weight: 700;
}

.sideNavigationBar a:hover {
	color: white;
}

.sideNavigationBar .closeButton {
	position: absolute;
	top: 10px;
	right: 25px;
	font-size: 20px;
	margin-left: 50px;
}

.line {
	display: flex;
	justify-content: space-between;
	align-items: center;
	margin: 2% 5%;
}

.line .side1 {
	padding-right: 50px;
}

.side1 h1 {
	font-size: 60px;
	margin-bottom: 10px;
	color: rgb(28, 203, 174);
}

.side1 button {
	width: 200px;
	padding: 12px 20px;
	border-radius: 20px;
	border-style: none;
	color: rgb(132, 65, 65);
	font-size: 17px;
	font-weight: 600;
}

a {
	text-decoration: none;
	color: white;
}

/* Header content responsive */
@media screen and (max-width: 980px) {
	.side2 img {
		width: 350px;
	}

	.side1 h1 {
		font-size: 40px;
	}

	.side1 p {
		font-size: 17px;
	}

	.line {
		margin-top: 80px;
	}
}

@media screen and (max-width: 600px) {
	.side1 h1 {
		font-size: 35px;
	}

	.line {
		flex-direction: column;
	}

	.line .side1 {
		padding: 30px;
	}
}

/* section */

section .topic a {
	font-size: 25px;
	font-weight: 500;
	margin-bottom: 10px;
}

.about .boxes {
	display: flex;
	flex-wrap: wrap;
	justify-content: space-between;
}

.about .boxes .box {
	margin: 10px 20px;
	max-width: calc(100% / 3 - 50px);
	text-align: center;
	border-radius: 12px;
	padding: 30px 10px;
	box-shadow: 0 5px 10px rgb(254, 254, 254);
	cursor: default;
}

/* Contact Page */

.contact {
	padding: 20px;
}

.contact .content {
	margin: 0 auto;
	padding: 30px 0;
}

.content .title {
	width: 80%;
	text-align: center;
	font-weight: bolder;
	font-size: 40px;
}

.title {
	margin-bottom: 30px;
	margin-left: 80px;
}

.contactMenu {
	display: flex;
	justify-content: space-evenly;
}

.input2 {
	margin-top: 10;
}

.label1 {
	font-size: 18px;
	margin-top: 8px;
	margin-bottom: 8px;
	font-weight: bolder;
}

.contactMenu .input1 input {
	border-radius: 13px;
	padding: 6px;
}

.input2 input {
	border-color: rgb(252, 244, 244);
	width: 400px;
}

.button {
	margin-top: 12px;
	margin-left: 5px;
}

.button button {
	width: 162px;
	height: 35px;
	border-radius: 12px;
	border-color: transparent;
}

.button button:hover {
	background-color: #8cc099;
}

button {
	width: 162px;
	height: 35px;
	border-radius: 12px;
	border-color: transparent;
}

button:hover {
	background-color: #8cc099;
}

.rightside1 {
	display: flex;
	flex-direction: column;
	margin-left: 300px;
}

.title1 {
	font-size: 18px;
	margin-top: 8px;
	margin-bottom: 5px;
	font-weight: bolder;
}

.content1 {
	width: 450px;
	margin-top: 2px;
	color: rgb(132, 130, 130);
}

/* Footer */
footer {
	background: var(--primary-color);
	padding: 15px 0;
	text-align: center;
	font-family: "Poppins", sans-serif;
}

footer .footer span {
	font-size: 17px;
	font-weight: 400;
	color: var(--white-color);
}

footer .footer span a {
	font-weight: 500;
	color: var(--white-color);
}

footer .footer span a:hover {
	text-decoration: underline;
}

@media screen and (max-width: 1060px) {
	.contactMenu {
		flex-direction: column;
		align-items: center;
	}

	.rightside1 {
		display: flex;
		flex-direction: column;
		margin-left: 0px;
	}

	.content1 {
		width: 100%;
		margin-top: 2px;
		color: rgb(131, 131, 131);
	}

	.side2 img {
		width: 95%;
		height: 90%;
	}
}

@media screen and (max-width: 600px) {
	.side2 img {
		width: 100%;
	}

	section .topic a {
		font-size: 20px;
	}

	section .topic p {
		font-size: 5px;
	}

	.about .boxes {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.about .boxes .box {
		max-width: 70%;
	}
}

JS

function openNavbar() {
	document.getElementById("sideNavigationBar")
		.style.width = "50%";
}
function closeNavbar() {
	document.getElementById("sideNavigationBar")
		.style.width = "0%";
}
