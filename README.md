# just-it-training
html
/*This is my css file*/


/*Global styles*/

ul {
    
    margin: 0;
    padding: 0;
}

h1 {
    
    font-size: 1.5em;
    text-align: center;
    font-family: 'Roboto', sans-serif;
    font-weight: lighter;
}


body {
    
    font-family: 'Ek Mukta', sans-serif;
    font-size: 1em;
    width: 100%;
    margin: 0;
    padding: 0;
    overflow-x: hidden;
}


/*-------------------------------------*/


/*Embeded fonts*/

@font-face {
    font-family: salesFont;
    src: url(../CaseStudy1/embedFonts/HelsinkiXXL-Black.eot);
}

@font-face {
    font-family: salesFont;
    src: url(../CaseStudy1/embedFonts/HelsinkiXXL-Black.woff);
}


.bgImage {
    
    position: relative;
    background-image: url(../CaseStudy1/img/prettyWoman.jpg);
    background-repeat: no-repeat;
    background-position: center 0;
    background-size: cover;
    width: 100% !important;
    height: 100vh;
    border-bottom: 15px solid rgba(54, 91, 70, 0.8);
    background-attachment: fixed;
}

.container {
    
    width: 80%;
    height: 100%;
    margin: 200px auto;
}

.logoC {

    position: absolute;
    top: 60px;
    left: 250px;
}

.logo {
    
}

/*Navigation styles*/

.navC {
    
    width: 50%;
    background-color: rgba(54, 91, 70, 0.95);
    padding: 15px 0 15px 51%;
    position: fixed;
    border-bottom: 3px solid rgba(54, 91, 70, 1);
    z-index: 1000;
    opacity: 1;
    background-image: url(../CaseStudy1/img/logo1.png);
    background-attachment: fixed;
    background-repeat: no-repeat;
    background-position: 12% 2px;
    background-blend-mode:multiply;
    opacity: 0;
    transition: all 2s ease;
    transform: translateY(-100px);
    
}

.navShowing{
    opacity: 1;
    transition: all 2s ease;
    transform: translateY(0);
}


nav a {
    
    font-family: 'Roboto', sans-serif;
    font-size: 0.8em;
    letter-spacing: 1px;
    color: rgba(255, 255, 255, 0.7);
    text-transform: uppercase;
    font-weight: 700;
    text-decoration: none;
    padding: 10px 15px;
    transition: all 0.5s ease;
}

.current > a {
    
    color: rgba(255, 255, 255, 1); !important;
    background-color: rgba(0, 0, 0, 0.3);
    padding: 10px 15px;
    border-radius: 3px 3px 3px 3px;
    -moz-border-radius: 3px 3px 3px 3px;
    -webkit-border-radius: 3px 3px 3px 3px;
    transition: all 1s ease;
}

nav a:hover {

    color: rgba(255, 255, 255, 1);

}

nav li {
    
    float: left;
    display: inline;
    padding: 0 20px 0 20px;
}

.isShowing{
    opacity: 1;
    transform: translate(0);
}
.actionB {
    
    position: absolute;
    top: 70vh;
    left: 260px;
  
}
.actionB:hover~.hand {
    animation: point 2s infinite ease-in-out;
}

.newCollectionB {
    
    padding: 5px 20px;
    line-height: 20px;
    border-radius: 5px 5px 5px 5px;
    -moz-border-radius: 5px 5px 5px 5px;
    -webkit-border-radius: 5px 5px 5px 5px;
    border: 2px solid rgba(54, 91, 70, 0.6);
    background-color: rgba(54, 91, 70, 0.3);
    cursor: pointer;
    outline: none;
    -webkit-transition: background-color 1000ms ease-out;
    -moz-transition: background-color 1000ms ease-out;
    -o-transition: background-color 1000ms ease-out;
    -ms-transition: background-color 1000ms ease-out; 
    transition: background-color 1000ms ease-out;
}

.newCollectionB:hover {
    
    border: 2px solid rgba(54, 91, 70, 1);
    background-color: rgba(54, 91, 70, 0.8);
    color: white;
    -webkit-transition: background-color 1000ms ease-in;
    -moz-transition: background-color 1000ms ease-in;
    -o-transition: background-color 1000ms ease-in;
    -ms-transition: background-color 1000ms ease-in; 
    transition: background-color 1000ms ease-in;
}


.hand {
    
    position: absolute;
    top: 70vh;
    left: 420px;
    color: rgba(54, 91, 70, 0.8);
    margin: 0 0 0 20px !important;
}

@keyframes point{
    0%{left: 420px;}
    50%{left: 500px;}
    100%{left: 420}
}
@-webkit-keyframes point{
    0%{left: 420px;}
    50%{left: 500px;}
    100%{left: 420}
}
.mouse {
    position: absolute;
    display: block;
    top: 85%;
    left: 50%;
    width: 2px;
    height: 6px;
    margin: -30px 0 0 -1px;
    background: white;
    
}

.scrollD {
    position: relative;
    display: block;
    width: 30px;
    height: 45px;
    margin: 0 auto 20px;
    top: 90vh;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    border-radius: 5px;
    border: 2px solid rgba(54, 91, 70, 1);
    background-color: rgba(54, 91, 70, 0.5);
}

.scrollD:hover {
    
    border: 2px solid rgba(255, 255, 255, 0.6);
}

.fa-arrow-down {
    
    color: white;
    font-weight: lighter;
}






/* The Modal (background) */
.modal {
    display: none; /* Hidden by default */
    position: fixed; /* Stay in place */
    z-index: 1; /* Sit on top */
    padding-top: 65px; /* Location of the box */
    left: 0;
    top: 0;
    width: 100%; /* Full width */
    height: 100%; /* Full height */
    overflow: auto; /* Enable scroll if needed */
    background-color: rgb(0,0,0); /* Fallback color */
    background-color: rgba(0,0,0,0.4); /* Black w/ opacity */
}

/* Modal Content */
.modal-content {
    position: relative;
    background-color: rgba(255, 255, 255, 0.5);
    margin: auto;
    padding: 0;
    /*border: 1px solid #888;*/
    width: 70%;
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2),0 6px 20px 0 rgba(0,0,0,0.19);
    -webkit-animation-name: animatetop;
    -webkit-animation-duration: 0.4s;
    animation-name: animatetop;
    animation-duration: 0.4s;
}

/* Add Animation */
@-webkit-keyframes animatetop {
    from {
        top:-300px;
        opacity:0
    } 
    to {
        top:0;
        opacity:1
    }
}

@keyframes animatetop {
    from {
        top:-300px;
        opacity:0
    }
    to {
        top:0;
        opacity:1
    }
}

/* The Close Button */
.close {
    position: absolute;
    top: 0px;
    left: 830px;
    color: white;
    /*color: rgba(54, 91, 70, 1);*/
    font-size: 50px;
    font-weight: bold;
    z-index: 100;
    text-shadow: 2px 1px red;
   
}

.close:hover,
.close:focus {
    color: rgba(54, 91, 70, 0.5);
    text-decoration: none;
    cursor: pointer;
}

.modal-body {
    padding-bottom: 0 !important;
    margin-bottom: 0 !important;
}

/*The video Styles*/

.myVideo {
    
    position: relative;
    width: 100%;
    margin: 13px auto 4px auto !important;
   
    
}

/*Featured products*/

.featuredPText {
    
    text-align: center;
}

.featuredP {
    
    width: 80%;
    height: 100% !important;
    margin: 0 auto;
    padding: 20px 30px;
    column-count: 3;
    -webkit-column-count: 3;
    -moz-column-count: 3;
    -ms-column-count: 3;
    -o-column-count: 3;
}

.featuredPSales {
    
    width: 60%;
    height: 100% !important;
    margin: 0 auto 50px auto;
    padding: 20px 30px;
    float: left;
    column-count: 3;
    -webkit-column-count: 3;
    -moz-column-count: 3;
    -ms-column-count: 3;
    -o-column-count: 3;
}


.productBox {
    
    position: relative;
    display: block;
    width: 90%;
    text-align: center;
    opacity: 1;
    transform: translate(0);

}

.sales {
    
    width: 80%;
    height: 100%;
    margin: 200px auto;
    padding: 0 0 100px 0;
    overflow: auto;
}

.productSales {
    
    position: relative;
    display: block;
    
    text-align: center;
}

.productSales img {
    
    position: relative;
    width: 80%;
    border: 5px solid rgba(54, 91, 70, 0.1);
}


.shoppingB {
    
    width: 30%;
    float: left;
    margin: 20px 0 0 0;
    border: 1px solid #ccc;
    height: 204px;
}

.shoppingText {
    
    font-family: salesFont;
    text-align: center;
    margin-left: 20px;
    float: none !important;
}

.deliveryO {
    
    width: 80%;
    margin: 0 auto;
    padding: 30px 10% 30px 20px;
    border: 1px solid #ccc;
    cursor: pointer;
    clear: both;
}


.productBox img {
    
    position: relative;
    width: 100%;
}


.productBox a {

    position: relative;
    color: inherit;
    text-decoration: none;
    display: block;
    cursor: pointer!important;
    overflow: hidden !important;

}



.pDetail {
    
    font-size: 0.8em;
    margin: 0 auto;
    padding: 0 25px;

}


figcaption > strong.price {
    
    display: block;
}

/*.isShowing {
    
    opacity: 1; 
    transform: translateX(0); 
}*/



/* Style the accordion panel. Note: hidden by default */
div.deliveryForm {
    margin: 0 10%;
    padding: 0 18px;
    background-color: white;
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.2s ease-out;
}

.deliveryO:after {
    content: '\002B';
    color: #777;
    font-weight: bold;
    float: right;
    font-size: 1em;
}

.deliveryO.active:after {
    content: "\2212";
}


/*The about page styles*/

.aboutText {
    
    column-count: 2;
    column-gap: 150px;
}

.aboutText img {
    
    text-align: right;
    margin: 20px auto 0 auto;
    border-radius: 5px 5px 5px 5px;
    -moz-border-radius: 5px 5px 5px 5px;
    -webkit-border-radius: 5px 5px 5px 5px;
}


/*My styles for the contact form*/

.formC {
    
    width: 45%;
    float: left;
    margin: 0 10% 150px 0;
    display: block;
}

.ourLocation {
    
    width: 40%;
    float: left;
    border: 1px solid #ccc;
    height: 297px;
    margin-top: 30px;
}

.sendB {
    
    font-size: 1em;
    color: #142b1b;
    /*padding: 5px 20px;*/
    line-height: 30px;
    border-radius: 5px 5px 5px 5px;
    -moz-border-radius: 5px 5px 5px 5px;
    -webkit-border-radius: 5px 5px 5px 5px;
    border: 2px solid rgba(0, 0, 0, 0.2);
    background-color: rgba(54, 91, 70, 0.6);
}

.sendB:hover {
    
    cursor: pointer;
    border: 2px solid rgba(54, 91, 70, 1);
    background-color: rgba(54, 91, 70, 0.8);
    color: white;
}

.socialMedia {
    
    height: 30px;
    text-align: center;
    color: white;
    padding: 20px 0 0 0;
    margin: 0 auto;
    width: 80%;
}

.logoSpace {
    
    margin: 0 20px;
}

.ourAddress {
    
    font-size: 0.8em;
    color: white;
    width: 80%;
    margin: 0 auto;
    padding: 20px 0;
    text-align: center;
}

.inputFields {
    
    width: 100%;
    outline: none;
    margin-bottom: 20px;
    padding-left: 10px;
}

footer {
    
    background-color: black;
    clear: both;
    margin: 0 auto;
    border-bottom: 15px solid rgba(54, 91, 70, 0.3);
}

