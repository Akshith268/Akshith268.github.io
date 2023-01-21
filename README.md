<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>home page</title>
    <style>
        body{
            margin: 0px;
            padding: 0px;
            height: 1000px;
        }
        nav{
            background-color:rgba(128, 0, 128, 0.575);
            color: black;
            font-family: monospace;
            font-size: 20px;
            font-weight: bolder;
            text-decoration: none;
            border-radius: 4px;
            position: relative;
            padding: 4px;
        }
        .searching{
            padding-inline-start: 500px;
        }
        .navbar input{
            border-radius: 5px;
            padding: 6px;
        }
        .navbar ul{
            overflow: auto;
        }
        .navbar li{
            float: left;
            list-style: none;
            padding-inline-end: 50px;
        }
        .under li a:hover, .under li a.active{
            transition: 0.3s;
            text-decoration: underline;
            color: white;
        }
        h1{
            padding-top: 250px;
            color: black;
            height: 500px;
            margin: auto;
            font-size: 70px;
            font-weight:bolder;
        }
        .heading{
            margin: 50px 22px;
            padding-left: 330px;
            border: 2px thin lightpink;
            border-radius: 12px;
            height: 500px;
            background-repeat: no-repeat;
            background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSnA6nlRkcWkIWaaUgt-6eH0Y8FRJIHX6cFyQ&usqp=CAU');
           background-color: lightpink;
            background-size: 100% 100%;
            opacity: calc(1);
        }
        h2{
            color: black;
            font-weight: bolder;
            font-size: 40px;
            padding-left: 560px;
            font-weight: bolder;
        }
        .heading1{
            text-align: center;
            font-size: 50px;
            font-family: monospace;
            background-repeat: no-repeat;
            background-size: 100% 100%;
            background-attachment: scroll;
            border: 2px thin #6e4f8f;
            border-radius: 12px;
            font-style: italic;
            font-weight: bolder;

        }
        .services{
           margin-left: 100px;
           margin-right: 100px;
           text-align: center;
           font-size: 30px;
        }
        .service{
            margin-left: 100px;
            margin-right: 100px;
            background-color: lightblue;
            border-radius: 9px;
            font-style: italic;
            font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        }
        .selecting{
               color: black;
                text-align: center;
               border: 2px solid black;
               margin-left: 300px;
               margin-right: 300px;
               text-transform: uppercase;
               text-decoration: none;
               font-size: 50px;

        }
        .selecting :hover{
            color: green;
            transition: 0.3s;
            background-color: black;
        }
    
        html,body{
    padding: 10px 0 0 0;
    margin: 0;
}
.galleryContainer{
    width: 100%;
    height: 700px;
    max-width: 1500px;
    margin: auto;
    user-select: none;
    box-shadow: 0px 0px 3px 1px #00000078;
    padding: 10px;
    box-sizing: border-box;
}
.galleryContainer .slideShowContainer{
    width: 100%;
    height: 90%;
    overflow: hidden;
    background-color: gainsboro;
    position: relative;
}
.galleryContainer .slideShowContainer #playPause{
    width: 32px;
    height: 32px;
    position: absolute;
    background-image: url(images/playPause.png);
    background-repeat: no-repeat;
    z-index: 5;
    background-size: cover;
    margin: 5px;
    cursor: pointer;
}
.galleryContainer .slideShowContainer #playPause:hover{
    opacity: .7;
}
.galleryContainer .slideShowContainer .imageHolder{
    width: 100%;
    height: 100%;
    position: absolute;
    opacity: 0;
}
.galleryContainer .slideShowContainer .imageHolder img{
    width: 100%;
    height: 100%;
}
.galleryContainer .slideShowContainer .imageHolder .captionText{
    display: none;
}

.galleryContainer .slideShowContainer .leftArrow,.galleryContainer .slideShowContainer .rightArrow{
    width: 50px;
    background: #00000036;
    position: absolute;
    left: 0;
    z-index: 1;
    transition: background 0.5s;
    height: 72px;
    top: 50%;
    transform: translateY(-50%);
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
}
.galleryContainer .slideShowContainer .rightArrow{
    left: auto;
    right: 0;
    border-top-right-radius: 0px;
    border-bottom-right-radius: 0px;
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
}
.galleryContainer .slideShowContainer .leftArrow:hover,.galleryContainer .slideShowContainer .rightArrow:hover{
    background: #000000a8;
    cursor: pointer;
}
.galleryContainer .arrow{
    display: inline-block;
    border: 3px solid white;
    width: 10px;
    height: 10px;
    border-left: none;
    border-bottom: none;
    margin: auto;
    position: absolute;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0;
}
.galleryContainer .arrow.arrowLeft{
    transform: rotateZ(-135deg);
}
.galleryContainer .arrow.arrowRight{
    transform: rotateZ(45deg);
}


.galleryContainer .slideShowContainer>.captionTextHolder{
    position: absolute;
    bottom: 0;
    z-index: 1;
    color: white;
    font-family: sans-serif;
    font-size: 20px;
    text-align: center;
    width: 100%;
    background: #00000047;
    height: 50px;
    line-height: 50px;
    overflow: hidden;
}
.galleryContainer .slideShowContainer>.captionTextHolder>.captionText{
    margin: 0;
}

.galleryContainer #dotsContainer{
    width: 100%;
    height: 10%;
    text-align: center;
    padding-top: 20px;
    box-sizing: border-box;
}
.galleryContainer #dotsContainer .dots{
    display: inline-block;
    width: 15px;
    height: 15px;
    border-radius: 50%;
    margin-left: 5px;
    background-color: #bbb;
    cursor: pointer;
    transition:background-color 0.5s;
}
.galleryContainer #dotsContainer .dots:first-child{
    margin-left: 0;
}
.galleryContainer #dotsContainer .dots:hover,.galleryContainer #dotsContainer .dots.active{
    background-color: #717171;;
}




.galleryContainer .moveLeftCurrentSlide{
    animation-name: moveLeftCurrent;
    animation-duration: 0.5s;
    animation-timing-function: linear;
    animation-fill-mode:forwards;

}
.galleryContainer .moveLeftNextSlide{
    animation-name: moveLeftNext;
    animation-duration: 0.5s;
    animation-timing-function: linear;
    animation-fill-mode:forwards;
}
@keyframes moveLeftCurrent {
    from {margin-left: 0;opacity: 1;}
    to {margin-left: -100%;opacity: 1;}
}
@keyframes moveLeftNext {
    from {margin-left: 100%;opacity: 1;}
    to {margin-left: 0%;opacity: 1;}
}


.galleryContainer .moveRightCurrentSlide{
    animation-name: moveRightCurrent;
    animation-duration: 0.5s;
    animation-timing-function: linear;
    animation-fill-mode:forwards;
}
.galleryContainer .moveRightPrevSlide{
    animation-name: moveRightPrev;
    animation-duration: 0.5s;
    animation-timing-function: linear;
    animation-fill-mode:forwards;
}
@keyframes moveRightCurrent {
    from {margin-left: 0;opacity: 1;}
    to {margin-left: 100%;opacity: 1;}
}
@keyframes moveRightPrev {
    from {margin-left: -100%;opacity: 1;}
    to {margin-left: 0%;opacity: 1;}
}
.slideTextFromBottom {
    animation-name: slideTextFromBottom;
    animation-duration: 0.7s;
    animation-timing-function: ease-out;
}
@keyframes slideTextFromBottom {
    from {opacity: 0;margin-top: 100px}
    to {opacity: 1;margin-top: 0px;}
}
.slideTextFromTop {
    animation-name: slideTextFromTop;
    animation-duration: 0.7s;
    animation-timing-function: ease-out;
}
@keyframes slideTextFromTop {
    from {opacity: 0;margin-top: -100px}
    to {opacity: 1;margin-top: 0px;}
}
        
    </style>
</head>

<header class="navbar">
    <nav>
        <ul class="under">
            <li><a class="active" href="/">HOME</a></li>
            <li><a href="">LEARN</a></li>
            <li><a href="">CONTACT US</a></li>
            <li><a href="./loginpage.html">LOGIN</a></li>
            <li class="searching">
                search:<input type="text" name="search" id="search" placeholder="search here">
            </li>
        </ul>
    </nav>
</header>
<body>
    <br><br>
    <div class="galleryContainer">
        <div class="slideShowContainer">
            <div id="playPause" onclick="playPauseSlides()"></div>
            <div onclick="plusSlides(-1)" class="nextPrevBtn leftArrow"><span class="arrow arrowLeft"></span></div>
            <div onclick="plusSlides(1)" class="nextPrevBtn rightArrow"><span class="arrow arrowRight"></span></div>
            <div class="captionTextHolder"><p class="captionText slideTextFromTop"></p></div>
            <div class="imageHolder">
                <img src="books.png">1366X768
                <p class="captionText">Caption Text-01</p>
            </div>
            <div class="imageHolder">
                <img src="books4.jpg">
                <p class="captionText">Caption Text-02</p>
            </div>
            <div class="imageHolder">
                <img src="books6.jpg">
                <p class="captionText">Caption Text-03</p>
            </div>
            <div class="imageHolder">
                <img src="books7.jpg">
                <p class="captionText">Caption Text-04</p>
            </div>
        </div>
        <div id="dotsContainer"></div>
    </div>
      <div class="heading">
        <h1 >
            FOCUS
            <span class="dot">.</span>
            STUDY
            <span class="dot">.</span>
            DEVELOP
        </h1>
    </div>
   <div class="service"> 
    <div>
        <div class="heading1">
            SERVICES
        </div>
        <p class="services">
            IT IS A TYPE OF E-LIBRARY WHICH IS USED IN A REAL TIME LIBRARY WHERE ONE CAN FIND THE BOOKS POSITION
            IN A LIBRARY.
        </p>
   </div>
   </div>

    <div class="selecting" >
            <a href="./loginpage.html">studentlogin</a>
    </div>
    <script>

var slideIndex,slides,dots,captionText;
function initGallery(){
    slideIndex = 0;
    slides=document.getElementsByClassName("imageHolder");
    slides[slideIndex].style.opacity=1;

    captionText=document.querySelector(".captionTextHolder .captionText");
    captionText.innerText=slides[slideIndex].querySelector(".captionText").innerText;

    //disable nextPrevBtn if slide count is one
    if(slides.length<2){
        var nextPrevBtns=document.querySelector(".leftArrow,.rightArrow");
        nextPrevBtns.style.display="none";
        for (i = 0; i < nextPrevBtn.length; i++) {
            nextPrevBtn[i].style.display="none";
        }
    }

    //add dots
    dots=[];
    var dotsContainer=document.getElementById("dotsContainer"),i;
    for (i = 0; i < slides.length; i++) {
        var dot=document.createElement("span");
        dot.classList.add("dots");
        dotsContainer.append(dot);
        dot.setAttribute("onclick","moveSlide("+i+")");
        dots.push(dot);
    }
    dots[slideIndex].classList.add("active");
}
initGallery();
function plusSlides(n) {
    moveSlide(slideIndex+n);
}
function moveSlide(n){
    var i;
    var current,next;
    var moveSlideAnimClass={
          forCurrent:"",
          forNext:""
    };
    var slideTextAnimClass;
    if(n>slideIndex) {
        if(n >= slides.length){n=0;}
        moveSlideAnimClass.forCurrent="moveLeftCurrentSlide";
        moveSlideAnimClass.forNext="moveLeftNextSlide";
        slideTextAnimClass="slideTextFromTop";
    }else if(n<slideIndex){
        if(n<0){n=slides.length-1;}
        moveSlideAnimClass.forCurrent="moveRightCurrentSlide";
        moveSlideAnimClass.forNext="moveRightPrevSlide";
        slideTextAnimClass="slideTextFromBottom";
    }

    if(n!=slideIndex){
        next = slides[n];
        current=slides[slideIndex];
        for (i = 0; i < slides.length; i++) {
            slides[i].className = "imageHolder";
            slides[i].style.opacity=0;
            dots[i].classList.remove("active");
        }
        current.classList.add(moveSlideAnimClass.forCurrent);
        next.classList.add(moveSlideAnimClass.forNext);
        dots[n].classList.add("active");
        slideIndex=n;
        captionText.style.display="none";
        captionText.className="captionText "+slideTextAnimClass;
        captionText.innerText=slides[n].querySelector(".captionText").innerText;
        captionText.style.display="block";
    }

}
var timer=null;
function setTimer(){
    timer=setInterval(function () {
        plusSlides(1) ;
    },6000);
}
setTimer();
function playPauseSlides() {
    var playPauseBtn=document.getElementById("playPause");
    if(timer==null){
        setTimer();
        playPauseBtn.style.backgroundPositionY="0px"
    }else{
        clearInterval(timer);
        timer=null;
        playPauseBtn.style.backgroundPositionY="-33px"
    }
}
     </script>

  
</body>
</html>
