
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> ATTRACT TOURISM WEBSITE</title>
<style>

    body{
        background-color: #eebdf5
    }
    @import url('https://fonts.googleapis.com/css2?family=Kalam:wght@300;400;700&display=swap');

*{
  font-family: 'Kalam', cursive;
  padding: 0; margin: 0;
  box-sizing: border-box;
  text-decoration: none;
  text-transform: capitalize;
}

html{
  overflow-x: hidden;
  font-size: 62.5%;
}
/*  DropDOnw Mneu Start  */
/*  DropDOnw Mneu Start  */
.navbar ul li{
    position: relative;
    border-radius: 23px;
}
.navbar ul li ul{
    position: absolute;
    display: inline ;
    left: 0;
    top: 100%;
    height: 250px;
    width: 200px;
    background-color: #f5ebf3;
    border-top: 1px solid #ddd;
    border-radius: 8px;
    transition: .1s;
}
.navbar ul li ul li{
    display: block;
    margin-left: 0;
}
.navbar ul li ul li a{
    display: block;
    border: none;
    margin: 10px;
    border-bottom: 1px solid #ddd;
}
.navbar ul ul li:first-child a{
    border-left: none;
}




/* hoaver */
.navbar ul li ul{
    opacity: 0;
    visibility: hidden;

    transform: scaleY(0);
    transform-origin: top center;
}
.navbar ul li:hover ul{
    transform: scaleY(1);
    opacity: 1;
    visibility: visible;
}

.navbar ul li ul li a:hover{}

.heading{
  color:#333;
  font-size: 3.5rem;
  padding: 1rem;
  padding-top: 6rem;
  text-align: center;
  letter-spacing: .2rem;
}

.heading span{
  color:#0098a1;
}

header{
  width: 96%;
  background:#fff;
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: fixed;
  top:1.5rem; left:50%;
  transform: translateX(-50%);
  border-radius: .5rem;
  box-shadow: 0 .3rem .5rem rgba(0,0,0,.3);
  padding:.3rem 2rem;
  transition: .2s linear;
  z-index: 1000;
}

.header-active{
  top:0;
  width:100%;
  border-radius: 0;
}

header .logo{
  color:#333;
  font-size: 3rem;
}

header .logo span{
  color:#0098a1;
}

header .navbar ul{
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin:0; padding:0;
}

header .navbar ul li{
  margin:0 1rem;
}

header .navbar ul li a{
  font-size: 2rem;
  color:#333;
  transition: .2s linear;
}


header .navbar ul li .active,
header .navbar ul li a:hover{
  color: #0098a1;
}

header .fa-bars{
  font-size: 3rem;
  color:#0098a1;
  cursor: pointer;
  display: none;
}

.home{
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: space-around;
  position: relative;
  padding:2rem 10rem;
}

.home .video video{
  position: absolute;
  top:0; left:0;
  height:100%;
  width: 100%;
  object-fit: cover;
  z-index: -1;
}

.home .content{
  /* margin-top: 7rem; */
}

.home .content h2{
  /* font-size: 6.1vw;
  color:#fff;
  text-shadow: 0 .3rem .5rem #000; */
  font-size: 50px;

}
/* 
.home .content p{
  font-size: 1.5vw;
  color:#eee;
  text-shadow: 0 .3rem .5rem #000;
  padding-left: 2rem;
  border-left: .3rem solid #ddd;
} */

.home .form-container form{
  margin-top: 8rem;
  padding:2rem;
  width:40rem;
  background-color: #fff;
  box-shadow: 0 .3rem .5rem rgba(0,0,0,.9);
  border-radius: .5rem;
}

.home .form-container form h3{
  color:#333;
  font-size: 3rem;
  text-align: center;
}

.home .form-container form span{
  color:#0098a1;
  font-size: 2.5rem;
  margin:.5rem 0;
  display: block;
}

.home .form-container form input{
  width: 100%;
  padding:0 1rem;
  height:4rem;
  font-size: 1.5rem;
  background:#eee;
  border:none;
  outline: none;
  color:#333;
  box-shadow: 0 .1rem .3rem rgba(0,0,0,.3) inset;
  border-radius: .5rem;
}

.home .form-container form input[type="submit"]{
  width:10rem;
  color:#fff;
  background:#0098a1;
  cursor: pointer;
  font-size: 2rem;
  margin-top: 2rem;
  transition: .2s linear;
}

.home .form-container form input[type="submit"]:hover{
  border:.2rem solid #0098a1;
  color:#0098a1;
  background: none;
}

.feature{
  min-height:100vh;
  background:#f9f9f9;
}

.feature .card-container{
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  width: 100%;
}

.feature .card-container .card{
  width:30rem;
  margin:2rem;
  background: #fff;
  border-radius: .5rem;
  box-shadow: 0 .3rem .5rem rgba(0,0,0,.3);
  overflow: hidden;
  position: relative;
}

.feature .card-container .card img{
  height:25rem;
  width: 100%;
  object-fit: cover;
}

.feature .card-container .content{
  padding-bottom: 2rem;
  text-align: center;
}

.feature .card-container .content .title{
  color:#0098a1;
  font-size: 3rem;
}

.feature .card-container .content p{
  color:#333;
  font-size: 1.3rem;
  padding:1rem;
}

.feature .card-container .content .stars i{
  padding:0 .2rem;
  font-size: 2rem;
  color:gold;
}

.feature .card-container .content .btn{
  font-size: 1.7rem;
  margin-top: 1.4rem;
  height:3.5rem;
  width:12rem;
  border-radius: .5rem;
  outline: none;
  border:none;
  background: #0098a1;
  color:#fff;
  cursor: pointer;
  transition: .2s linear;
}

.feature .card-container .content .btn:hover{
  background: none;
  border:.2rem solid #0098a1;
  color:#0098a1;
}

.feature .card-container .card .discount{

  /* top:1rem; left: 1rem; */
  /* display: block; */
  height:3.5rem;
  width:6rem;
  background: #f598ed;
  color:#fff;
  line-height: 4rem;
  text-align: center;
  font-size: 2rem;
}

.about{
  min-height: 100vh;
}

.about .row{
  display: flex;
  align-items: center;
  justify-content: space-around;
  width:90%;
  margin:0 auto;
}

.about .row .image img{
  height:65vh;
  width: 50vw;
}

.about .row .content h3{
  font-size: 4rem;
  color:#0098a1;
}

.about .row .content p{
  font-size: 1.9rem;
  color:#333;
}

.about .row .content .btn{
  outline: none;
  border:none;
  cursor: pointer;
  transition: .2s linear;
  height:4rem;
  width:18rem;
  margin-top: 1rem;
  color:#fff;
  background: #0098a1;
  font-size: 2rem;
}

.about .row .content .btn1,
.about .row .content .btn:hover{
  background: none;
  color:#0098a1;
  border:.2rem solid #0098a1;
  margin-right: 1rem;
}

.gallery{
  min-height: 100vh;
}

.gallery .box-container{
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  width: 90%;
  margin:0 auto;
}

.gallery .box-container .box{
  height:20rem;
  width:30rem;
  margin:2rem;
  cursor: pointer;
  overflow: hidden;
  position: relative;
}

.gallery .box-container .box img{
  height:100%;
  width:100%;
  object-fit: cover;
}

.gallery .box-container .box .icons{
  position: absolute;
  top:120%; left: 0;
  background:linear-gradient(transparent, #333);
  display: flex;
  align-items: flex-end;
  justify-content: space-around;
  height:100%;
  width: 100%;
  opacity: 0;
  transition: .2s linear;
}

.gallery .box-container .box:hover .icons{
  opacity: 1;
  top:0;
}

.gallery .box-container .box .icons a{
  color:#fff;
  text-shadow: 0 .1rem .3rem #000;
  font-size: 3rem;
  padding-bottom: 2rem;
}

.gallery .box-container .box .icons a:hover{
  color:#0098a1;
}

.review{
  background: url(../images/review-bg.jpg), linear-gradient(#0098a1, #0098a1) no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  background-blend-mode: multiply;
}

.review .heading{
  color:#fff;
  padding-bottom: 4rem;
}

.review .heading span{
  color:gold;
}

.review .box-container{
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

.review .box-container .box{
  width:35rem;
  margin:4rem 2rem;
  padding-bottom: 2rem;
  text-align: center;
  box-shadow: 0 .3rem .5rem #000;
  background:#fff;
}

.review .box-container .box .image{
  margin-top: -5rem;
}

.review .box-container .box .image img{
  height:10rem;
  width:10rem;
  border-radius: 50%;
  object-fit: cover;
  border: .7rem solid #fff;
}

.review .box-container .box .content h3{
  font-size: 2rem;
  color:#0098a1;
}

.review .box-container .box .content p{
  font-size: 1.4rem;
  color:#333;
  padding:.5rem 1.5rem;
}

.review .box-container .box .content .stars i{
  color:gold;
  font-size: 1.7rem;
  padding:1rem .1rem;
}

.contact .row{
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.contact .row .contact-info .box{
  margin:4rem 2rem;
}

.contact .row .contact-info .box h3{
  font-size: 2rem;
  color:#333;
}

.contact .row .contact-info .box h3 i{
  color:#0098a1;
}

.contact .row .contact-info .box p{
  padding-left: 3rem;
  font-size: 1.7rem;
  color:#aaa;
}

.contact .row .contact-form-container{
  width:50%;
}

.contact .row .contact-form-container h3{
  font-size: 4rem;
  padding-top: 4rem;
  color:#0098a1;
} 

.contact .row .contact-form-container .inputBox{
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

.contact .row .contact-form-container .inputBox input{
  width: 49%;
}

.contact .row .contact-form-container form input, textarea{
  outline: none;
  border:.2rem solid #0098a1;
  height:4rem;
  background:#fff;
  padding:0 1rem;
  margin:1rem 0;
  font-size: 1.8rem;
}

.contact .row .contact-form-container form textarea{
  width:100%;
  padding:1rem;
  resize: none;
  height:20%;
}

.contact .row .contact-form-container form input[type="submit"]{
  color:#0098a1;
  border:.2rem solid #0098a1;
  cursor: pointer;
  transition: .2s;
  width:20rem;
}

.contact .row .contact-form-container form input[type="submit"]:hover{
  color:#fff;
  background:#0098a1;
}

.newsletter{
  padding:2rem;
  background:linear-gradient(rgba(0,0,0,.6),rgba(0,0,0,.6)), url(../images/img5.jpg) no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  text-align: center;
}

.newsletter h1{
  font-size: 5rem;
  color:#fff;
  text-shadow: 0 .3rem .5rem #000;
}

.newsletter p{
  font-size: 2rem;
  color:#eee;
  padding:1rem 15rem;
}

.newsletter form input{
  outline:none;
  border:none;
  height:5rem;
}

.newsletter form input[type="email"]{
  width:40rem;
  padding:0 1rem;
  color:#fff;
  background:rgba(255,255,255,.2);
  font-size: 2rem;
}

.newsletter form input[type="email"]::placeholder{
  color:#ccc;
}

.newsletter form input[type="submit"]{
  width:20rem;
  color:#fff;
  background:#0098a1;
  font-size: 2rem;
  cursor: pointer;
  margin-left: -1.1rem;
  transition: .2s;
}

.newsletter form input[type="submit"]:hover{
  border:.2rem solid #fff;
  color:#fff;
  background:none;  
}

.footer{
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding:2rem;
  background:#222;
}

.footer .credit{
  font-size: 2rem;
  color:#eee;
}

.footer .credit span{
  color:#0098a1;
}

.footer .icons a{
  font-size: 2rem;
  margin:0 .5rem;
  height:4rem;
  width:4rem;
  line-height: 3.5rem;
  text-align: center;
  border-radius: 50%;
  color:#fff;
  border:.2rem solid #fff;
  transition: .2s linear;
}

.footer .icons a:hover{
  background:#0098a1;
}



















/* media queries  */

@media (max-width:991px){

  .home{
    flex-flow: column;
    padding:1.5rem;
  }

  .home .content{
    text-align: center;
  }

  .home .content h1{
    font-size: 5.5rem;
  }

  .home .content p{
    font-size: 1.8rem;
    padding:0; 
    border:none;
  }

}

@media (max-width:768px){

  html{
    font-size: 55%;
  }

  header .fa-bars{
    display: block;
  }

  header .navbar{
    position: fixed;
    top:-100rem; left:50%;
    transform: translateX(-50%);
    width: 100%;
    background-color: #fff;
    border-radius: .5rem;
    box-shadow: 0 .3rem .5rem rgba(0,0,0,.3);
    z-index: 1000;
    transition: .2s linear;
    opacity: 0;
  }

  header .navbar ul{
    flex-flow: column;
  }

  header .navbar ul li{
    margin:1rem 0;
    width: 100%;
    text-align: center;
  }

  header .navbar ul li a{
    display: block;
    font-size: 3rem;
  }

  header .nav-toggle{
    top:5.5rem;
    opacity: 1;
  }

  .about .row{
    flex-flow: column;
  }

  .about .row .image img{
    width: 90vw;
  }

  .about .row .content{
    text-align: center;
  }

  .about .row .content .btn1{
    margin-right: 0;
  }

  .contact .row{
    flex-flow: column;
    align-items: flex-start;
  }

  .contact .row .contact-form-container{
    width:90%; 
    margin:0 auto;
  }

  .newsletter p{
    padding:1rem 0;
  }

  .newsletter form input[type="email"]{
    width: 100%;
    margin-bottom: 1rem;
  }

  .footer{
    flex-flow: column;
  }

  .footer .credit{
    text-align: center;
    padding-bottom: 3rem;
  }

}

@media (max-width:500px){

  .home .form-container{
    width: 100%;
  }

  .home .form-container form{
    width: 100%;
    margin:3rem 0;
  }

  .home .form-container form input[type="submit"]{
    width: 100%;
  }

  .contact .row .contact-form-container form input{
    margin:1rem 0;
    width:100%;
  }

  .contact .row .contact-form-container form input[type="submit"]{
    width:100%;
  }

}
.animation{
    background-repeat: no-repeat;
            background-size: 100% 100%;
            background-attachment: fixed;
            height: 400px;
}
</style>
   <script>
       $(document).ready(function(){
 $('.fa-bars').click(function(){
 $(this).toggleClass('fa-times');
 $('.navbar').toggleClass('nav-toggle');
 });
 $(window).on('load scroll',function(){
 $('.fa-bars').removeClass('fa-times');
 $('.navbar').removeClass('nav-toggle');
 if($(window).scrollTop() > 30){
 $('header').addClass('header-active');
 }else{
 $('header').removeClass('header-active');
 }
 $('section').each(function(){
 var id = $(this).attr('id');
 var height = $(this).height();
 var offset = $(this).offset().top - 200;
 var top = $(window).scrollTop();
 if(top >= offset && top < offset + height){
 $('.navbar ul li a').removeClass('active');
 $('.navbar').find('[data-scroll="' + id +
'"]').addClass('active');
 }
 });
 });
})
   </script>

</head>

<body>

<header>

<a href="#" class="logo">travel <span>.</span></a>

<nav class="navbar">
    <ul>
        <li><a data-scroll="home" href="#home" class="active">home</a></li>
        <li><a data-scroll="feature" href="#feature">feature</a></li>
        <li><a data-scroll="about" href="#about">about</a></li>
            <li><a data-scroll="about" href="#about" style="color: #fc05d2;">social media</a>
            <ul>
            <li> <a href="#">whatsapp</a></li>
            <li><a href="#">instagram</a></li>
            <li><a href="#">twiter</a></li>
            <li><a href="https://facebook.com" > facebook</a></li>
            <li><a href="#">DropDonw item</a></li>
            <li><a href="#">DropDonw item</a></li>
        </ul>
    </li>
        <li><a data-scroll="gallery" href="#gallery">gallery</a></li>
        <li><a data-scroll="review" href="#review">review</a></li>
        <li><a data-scroll="contact" href="#contact">contact</a></li>
    </ul>
</nav>

<div class="fas fa-bars"></div>

</header>


<section class="home" id="home">

<div class="video">
    <video src="images/video.mp4" loop muted autoplay></video>
</div>

<div class="content">
    <h2 style="background-color: #fdc9f9;color: #f817d3;border-radius: 10px;">antaheen bangla</h2>
    <!-- <p style="color: #442542;">we are so lucky because you are visited our sites its a great opprtunity to us to help you for explor our district</p> -->
</div>
<marquee  direction="right" class="animation">
    <img src="video/a.gif" width="22%">&emsp;&emsp;&emsp;
    <img src="video/b.gif" width="11%">&emsp;
    <img src="video/c (2).gif" width="4%">&nbsp;
</marquee>


<!-- <div class="form-container">
    <form action="">

        <H3> destination COOCHBEHAR </H3>n

        <span>location</span>
        <input type="text" placeholder="place you want to visit">

        <span>guest members</span>
        <input type="number" placeholder="number of peoples">

        <span>arrival</span>
        <input type="date">

        <span>leaving</span>
        <input type="date">

        <input type="submit" value="search">

    </form> -->


</section>



<section class="feature" id="feature">

<h1 class="heading"><span>f</span>eatured <span>l</span>ocations</h1>

<div class="card-container">

    <div class="card">
        <span class="discount">haa haa</span>
        <img src="IMG/YUVARAJ.jpeg" alt="">
        <div class="content">
            <h3 class="title"> YUVARAJ HOTEL </h3>
            <p>it is a luxary hotel and it is  a four flor hotel where you enjoying the whole trip with your familly</p>
            <div class="stars">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star-half-alt"></i>
            </div>
            <a href="https://youtu.be/3A3bWkCkGhg"><button class="btn">check out!</button></a>
        </div>
    </div>

    <div class="card">
        <img src="IMG/RAJBARI2.jpeg" alt="">
        <div class="content">
            <h3 class="title">COOCHBEHAR </h3>
            <p> this is our main tourist attraction pease come in cooch behar visit here</p>
            <div class="stars">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star-half-alt"></i>
            </div>
            <a href="#"><button class="btn">check out!</button></a>
        </div>
    </div>

    <div class="card">
        <span class="discount">-45%</span>
        <img src="IMG/ELLORA.jpeg" alt="">
        <div class="content">
            <h3 class="title"> HOTEL ELLORA </h3>
            <p>this is a best hotel where you stay this is in main town</p>
            <div class="stars">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star-half-alt"></i>
            </div>
            <a href="#"><button class="btn">check out!</button></a>
        </div>
    </div>

</div>

</section>




<section id="about" class="about">

<h1 class="heading"><span>a</span>bout <span>C</span>OOCHBEHAR</h1>

<div class="row">

    <div class="image">
        <img src="img/our office.jpeg" alt="">
    </div>

    <div class="content">
        <h3>&nbsp;&nbsp;&nbsp;why choose &nbsp;&nbsp;&nbsp;COOCHBEHAR?</h3>
        <p> &nbsp;&nbsp;&nbsp;COOCHBEHAR is a historical place here you all the &nbsp;&nbsp;&nbsp;historical monument and historical palace here &nbsp;&nbsp;&nbsp;you know the life style of rajbongshi people &nbsp;&nbsp;&nbsp;and&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; rajbongshi language also </p><br>
        <p>&nbsp;&nbsp;&nbsp; as well as you know  the more thing when you &nbsp;&nbsp;&nbsp;come to our COOCHBEHAR </p>
        &nbsp;&nbsp; <a href="#"><button class="btn btn1">read more</button></a>
        <a href="#"><button class="btn">get started</button></a>
    </div>

</div>

</section>




<section id="gallery" class="gallery">

<h1 class="heading"><span>g</span>allery</h1>

<div class="box-container">

    <div class="box">
        <img src="img/sagar dighi.jpeg" alt="">
        <div class="icons">
            <a href="#" class="fas fa-heart"></a>
            <a href="#" class="fas fa-share"></a>
            <a href="#" class="fas fa-search"></a>
        </div>
    </div>

    <div class="box">
        <img src="img/mdan mohan mandir.jpeg" alt="">
        <div class="icons">
            <a href="#" class="fas fa-heart"></a>
            <a href="#" class="fas fa-share"></a>
            <a href="#" class="fas fa-search"></a>
        </div>
    </div>

    <div class="box">
        <img src="img/baneshwar mandir.jpeg" alt="">
        <div class="icons">
            <a href="#" class="fas fa-heart"></a>
            <a href="#" class="fas fa-share"></a>
            <a href="#" class="fas fa-search"></a>
        </div>
    </div>

    <div class="box">
        <img src="img/mudra.jpeg" alt="">
        <div class="icons">
            <a href="#" class="fas fa-heart"></a>
            <a href="#" class="fas fa-share"></a>
            <a href="#" class="fas fa-search"></a>
        </div>
    </div>

    <div class="box">
        <img src="img/old images.jpeg" alt="">
        <div class="icons">
            <a href="#" class="fas fa-heart"></a>
            <a href="#" class="fas fa-share"></a>
            <a href="#" class="fas fa-search"></a>
        </div>
    </div>

    <div class="box">
        <img src="img/city mall.jpeg" alt="">
        <div class="icons">
            <a href="#" class="fas fa-heart"></a>
            <a href="#" class="fas fa-share"></a>
            <a href="#" class="fas fa-search"></a>
        </div>
    </div>

</div>

</section>



<section id="review" class="review">

<h1 class="heading"><span>the</span>peoples who visited coochbehar previous time</h1>


<div class="box-container">

    <div class="box">
        <div class="image">
            <img src="img/dayahang.jpeg" alt="">
        </div>
        <div class="content">
            <h3>Dayahang Rai</h3>
            <p>he is dayhang Rai who visited our COOCHBEHAR  and he said that  " coochbehar is a great historocal place it is great visited place of my life " </p>
            <div class="stars">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star-half-alt"></i>
            </div>
        </div>
    </div>

    <div class="box">
        <div class="image">
            <img src="img/dechen.jpeg" alt="">
        </div>
        <div class="content">
            <h3>Dechen Pem</h3>
            <p>he is Dechen Pem who visited our COOCHBEHAR  in 2020 and he said that  " the RAJBARI OF COOCHBEHAR is a beautifull place and he like the sagardighi of COOCHBEHAR" </p>
            <div class="stars">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star-half-alt"></i>
                <i class="far fa-star"></i>
            </div>
        </div>
    </div>

    <div class="box">
        <div class="image">
            <img src="img/siam2.jpeg" alt="">
        </div>
        <div class="content">
            <h3>Siam Ahmed</h3>
            <p>He is Siam Ahmed the great bangladeshi actor who visited our locality and enjoying the whole toor as his opinion the rajbongshi people are great and he said the people are very helpfull "  </p>
            <div class="stars">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star-half-alt"></i>
                <i class="far fa-star"></i>
            </div>
        </div>
    </div>

</div>

</section>



<section id="contact" class="contact">

<h1 class="heading"><span>c</span>ontact <span>u</span>s</h1>

<img src="img/map2.jpeg" width="100%" height="300" frameborder="0" style="border:0; outline:none;" allowfullscreen="" aria-hidden="false" tabindex="0"></img>

<div class="row">

<div class="contact-info">

    <div class="box">
        <h3> <i class="fas fa-home"></i> address </h3>
        <p>Cooch Behar <br>
        West Behar, <br>
        736179.</p>
    </div>

    <div class="box">
        <h3> <i class="fas fa-envelope"></i> e-mail </h3>
        <p>souradeep@gmail.com</p>
    </div>

    <div class="box">
        <h3> <i class="fas fa-phone"></i> phone </h3>
        <p>9547543**7</p>
    </div>

</div>

<div class="contact-form-container">

    <form action="">

        <h3>get in touch</h3>

        <div class="inputBox">
            <input type="text" placeholder="full name">
            <input type="email" placeholder="e-mail">
        </div>

        <textarea name="" id="" cols="30" rows="10" placeholder="message"></textarea>

        <input type="submit" value="message">

    </form>

</div>

</div>

</section>


<section class="newsletter">

<h1>sign up </h1>

<p>heiiii you! hurry up  sign up  the first 100 sign up will guide by our student group </p>

<form action="">
    <input type="email" placeholder="enter your email">
    <input type="submit" value="sign up">
</form>

</section>

<section class="footer">

<h1 class="credit">created by <span>souradeep singha</span></h1>

<div class="icons">
    <a href="#" class="fab fa-facebook-f"></a>
    <a href="#" class="fab fa-twitter"></a>
    <a href="#" class="fab fa-instagram"></a>
    <a href="#" class="fab fa-github"></a>
</div>

</section>

</body>
</html>

<!-- jquery cdn link  -->

<!-- <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script> -->

<!-- custom js file link  -->
<!-- <script src="js/main.js"></script> -->
