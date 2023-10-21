<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Banuja fashion designer</title>

    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css" />

    <!-- font awesome cdn link  -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">

    <!-- custom css file link  -->
    <link rel="stylesheet" href="style.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700&display=swap');

:root{
    --orange:#fc0303;
    --white-color:#db5353;
    --black-color:#000;
    --light-color:rgba(0,0,0,.3);
}

*{
    font-family: 'Roboto', sans-serif;
    margin:0; padding:0;
    box-sizing: border-box;
    outline: none; border:none;
    text-decoration: none;
    text-transform: capitalize;
    transition:.2s linear;
}

html{
    font-size: 62.5%;
    overflow-x: hidden;
    scroll-padding-top: 7.5rem;
    scroll-behavior: smooth;
}

html::-webkit-scrollbar{
    width:1rem;
}

html::-webkit-scrollbar-track{
    background:var(--white-color);
}

html::-webkit-scrollbar-thumb{
    background:var(--black-color);
    border-radius: 5rem;
}

body{
    background:url(./img/logo2.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}
@media (max-width: 520px){
    html{
      font-size: 50%;
    }
    #home{
      background: url(./img/logo2.jpg) no-repeat;
      
    
    }}

body.active{
    --white-color:#111;
    --black-color:#fff;
    --light-color:rgba(255,255,255,.3);
    background:#222;
}
.user h3{
    color: #ce7d0c;
}
section{
    padding:1rem 9%;
}

.heading{
    padding:1rem 0;
    margin-bottom: 2rem;
    border-bottom: .1rem solid var(--light-color);
    font-size: 3rem;
    color:var(--black-color);
    text-transform: uppercase;
}
.logo span{
    color: #fff;
}
.heading span{
    color:var(--orange);
    text-transform: uppercase;
}

.btn{
    display: inline-block;
    margin-top: 1rem;
    border-radius: 5rem;
    background: papayawhip;
    color:var(--white-color);
    font-size: 1.8rem;
    padding:.9rem 3.5rem;
    cursor: pointer;
}

.btn:hover{
    background:var(--orange);
    color:#fff;
}

header{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: var(--white-color);
    border-bottom: .1rem solid var(--light-color);
    padding:1.5rem 9%;
}

header .logo{
    text-transform: uppercase;
    font-weight: bolder;
    color:var(--black-color);
    font-size: 3rem;
}

header .logo span{
    color:var(--orange);
}

header form{
    display: flex;
    align-items: center;
    width: 40rem;
    border-radius: 5rem;
    height: 5rem;
    background: var(--black-color);
    overflow:hidden;
}

header form input{
    width: 100%;
    height: 100%;
    background: none;
    font-size: 1.7rem;
    color:var(--white-color);
    padding:0 2rem;
    text-transform: none;
}

header form label{
    font-size: 2rem;
    padding-right: 2rem;
    color:var(--white-color);
    cursor: pointer;
}

header form label:hover{
    color:var(--orange);
}

header .icons div,
header .icons a{
    height: 4rem;
    width: 4rem;
    font-size: 1.7rem;
    line-height: 4rem;
    background: var(--black-color);
    color:var(--white-color);
    text-align: center;
    border-radius: 50%;
    cursor: pointer;
    margin-right: .7rem;
}

header .icons div:hover,
header .icons a:hover{
    background: var(--orange);
    color:#fff;
    transform: rotate(360deg);
}

header.active{
    position: fixed;
    top:0; left: 0;
    z-index: 100;
}

.navbar{
    position: fixed;
    top:0; left: -120%;
    z-index: 1000;
    height: 100%;
    background: var(--white-color);
    padding:3rem;
    width: 30rem;
}

.navbar.active{
    left: 0;
    box-shadow: 0 0 0 100vw var(--light-color);
}

.navbar .user{
    text-align: center;
    margin:3rem auto;
}

.navbar .user img{
    height: 15rem;
    width: 15rem;
    border-radius: 50%;
    border:.5rem solid var(--white-color);
    object-fit: cover;
    box-shadow: 5rem 2rem 0 -3rem var(--orange),
                -5rem -2rem 0 -3rem var(--orange);
}

.navbar .user h3{
    padding-top: .5rem;
    color:var(--black-color);
    font-weight: 500;
    font-size: 2rem;
}

.navbar .links a{
    display: block;
    border-bottom: .1rem solid var(--light-color);
    font-size: 2rem;
    padding:1.5rem 0;
    color:var(--black-color);
}

.navbar .links a:last-child{
    border: none;
}

.navbar .links a:hover{
    letter-spacing: .2rem;
    color:var(--orange);
}

.navbar #close{
    position: absolute;
    top:1rem; right:2rem;
    font-size: 3rem;
    cursor: pointer;
    color:var(--black-color);
}

.navbar #close:hover{
    color: var(--orange);
}

.home{
    min-height: 90vh;
    display: flex;
    align-items: center;
    flex-wrap: wrap-reverse;
    gap:1.5rem;
}

.home .content{
    flex:1 1 40rem;
}

.home .image{
    flex:1 1 40rem;
    text-align: center;
}

.home .image img{
    width:30vw;
}

.home .content span{
    color:var(--orange);
    font-size: 3rem;
}

.home .content h3{
    color:var(--black-color);
    font-size: 8rem;
    text-transform: uppercase;
}

.category .box-container{
    display: flex;
    flex-wrap: wrap;
    gap:1.5rem;
}

.category .box-container .box{
    height: 30rem;
    flex:1 1 40rem;
    border-radius: .5rem;
    position: relative;
    overflow:hidden;
}

.category .box-container .box img{
    height: 100%;
    width: 100%;
    object-fit: cover;
}

.category .box-container .box:hover img{
    transform: scale(1.1);
}

.category .box-container .content{
    position: absolute;
    bottom: 7rem; left:2rem;
}

.category .box-container .content span{
    font-size: 2rem;
    color:var(--orange);
}

.category .box-container .content h3{
    font-size: 3rem;
    color:#fff;
    text-transform: uppercase;
    padding-top: .5rem;
}

.products .product-slider .slide{
    overflow: hidden;
    position: relative;
    border:.1rem solid var(--light-color);
    border-radius: .5rem;
    background: wheat;
}

.products .product-slider .slide .image{
    padding:1rem;
}

.products .product-slider .slide .image img{
    height: 50rem;
    width: 100%;
    object-fit: cover;
}

.products .product-slider .slide .content{
    padding:2rem;
    border-top: .1rem solid var(--light-color);
}

.products .product-slider .slide .icons{
    position: absolute;
    top:0; right:-7rem;
}

.products .product-slider .slide:hover .icons{
    right:1rem;
}

.products .product-slider .slide .icons a{
    height:5rem;
    width:5rem;
    line-height: 5rem;
    text-align: center;
    font-size: 2rem;
    border-radius: 50%;
    background: var(--black-color);
    color:var(--white-color);
    display: block;
    margin-top: 1rem;
}

.products .product-slider .slide .icons a:hover{
    background:var(--orange);
    color:#fff;
}

.products .product-slider .slide .content .stars i{
    font-size: 2rem;
    color:var(--orange);
}

.products .product-slider .slide .content .stars span{
    font-size: 2rem;
    color:var(--black-color);
    font-weight: 300;
}

.products .product-slider .slide .content h3{
    color:var(--black-color);
    font-weight: normal;
    font-size: 2.5rem;
    padding:.5rem 0;
}

.products .product-slider .slide .content .price{
    color:var(--orange);
    font-weight: bolder;
    font-size: 2.5rem;
    padding:.5rem 0;
}

.products .product-slider .slide .content .price span{
    color:var(--black-color);
    font-weight: normal;
    font-size: 1.5rem;
    text-decoration: line-through;
}

.products .product-slider .swiper-button-next,
.products .product-slider .swiper-button-prev{
    color:var(--black-color);
}

.products .gap{
    margin-bottom: 2rem;
}

.featured .box-container{
    display: flex;
    flex-wrap: wrap;
    gap:1.5rem;
}

.featured .box-container .box{
    flex:1 1 27rem;
    background: wheat;
    border:.1rem solid var(--light-color);
    border-radius: .5rem;
    padding:1rem;
}

.featured .box-container .box .image-container{
    display: flex;
    gap:1.5rem;
    align-items: center;
    padding:1rem;
}

.featured .box-container .box .image-container .small-image{
    width:20%;
}

.featured .box-container .box .image-container .big-image{
    width:80%;
}

.featured .box-container .box .image-container .small-image img{
    width:100%;
    padding: .5rem;
    margin-bottom: 1rem;
    border:.1rem solid var(--light-color);
    cursor: pointer;
}

.featured .box-container .box .image-container .big-image img{
    width:100%;
}

.featured .box-container .box .content{
    padding:1rem;
    border-top: .1rem solid var(--light-color);
}

.featured .box-container .box .content h3{
    font-size: 2.5rem;
    color:var(--black-color);
}

.featured .box-container .box .content .stars{
    padding: .5rem 0;
}

.featured .box-container .box .content .stars i{
    font-size: 1.5rem;
    color:var(--orange);
}

.featured .box-container .box .content .stars span{
    font-size: 1.5rem;
    color:var(--black-color);
    font-weight: 300;
}

.featured .box-container .box .content p{
    color:var(--black-color);
    font-size: 1.5rem;
    padding:.5rem 0;
}

.featured .box-container .box .content .price{
    color:var(--orange);
    font-size: 2.5rem;
    padding:.5rem 0;
    font-weight: bolder;
}

.featured .box-container .box .content .price span{
    color:var(--black-color);
    font-size: 1.5rem;
    text-decoration: line-through;
    font-weight: 300;
}

.deal .row{
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap:1.5rem;
    text-align: center;
    border:.1rem solid var(--light-color);
    background:wheat;
    border-radius: .5rem;
    padding:1rem;
}

.deal .row .content{
    flex:1 1 40rem;
    padding:1rem;
}

.deal .row .image{
    flex:1 1 40rem;
    padding:2rem;
}

.deal .row .image img{
    width:100%;
}

.deal .row .discount{
    font-size: 2rem;
    color:var(--orange);
}

.deal .row .text{
    font-size: 4rem;
    color:var(--black-color);
    padding:.5rem 0;
}

.deal .row .count-down{
    display: flex;
    gap:2rem;
    justify-content: center;
    padding:.5rem 0;
}

.deal .row .count-down h3{
    color:var(--orange);
    font-size: 4rem;
}

.deal .row .count-down span{
    color:var(--light-color);
    font-size: 1.5rem;
}

.review .review-slider .slide{
    background:wheat;
    border-radius: .5rem;
    border:.1rem solid var(--light-color);
    padding:2rem;
}

.review .review-slider .slide .stars{
    padding:1rem 0;
}

.review .review-slider .slide .stars i{
   font-size: 2rem;
   color:var(--orange);
}

.review .review-slider .slide p{
    color:var(--black-color);
    font-size: 1.6rem;
    font-weight: 300;
    line-height: 1.5;
    padding:1rem 0;
}

.review .review-slider .slide .user{
    padding-top: .5rem;
    display: flex;
    align-items: center;
}

.review .review-slider .slide .user img{
    margin-right: 1.5rem;
    height:7rem;
    width:7rem;
    border-radius: 50%;
    object-fit: cover;
}

.review .review-slider .slide .user h3{
    color:var(--black-color);
    font-size: 2.5rem;
}

.review .review-slider .slide .user span{
    color:var(--light-color);
    font-size: 1.7rem;
}

.footer .footer-container{
    background: #fff;;
    border:.1rem solid var(--light-color);
    border-radius: .5rem;
    padding:2rem;
}

.footer .footer-container .box-container{
    display: flex;
    flex-wrap: wrap;
}

.footer .footer-container .box-container .box{
    flex:1 1 25rem;
}

.footer .footer-container .box-container .box h3{
    color:black;
    font-size: 2.5rem;
    padding:1rem 0;
}

.footer .footer-container .box-container .box a{
    display: block;
    color:goldenrod;
    font-size: 1.7rem;
    padding:1rem 0;
    font-weight: 300;
}

.footer .footer-container .box-container .box a:hover{
    color:var(--orange);
}

.footer .footer-container .box-container .box img{
    margin-top: 1rem;
}

.footer .footer-container .credit{
    font-size: 2rem;
    margin-top: 2rem;
    padding-top: 2rem;
    border-top: .1rem solid var(--light-color);
    color:var(--black-color);
    text-align: center;
}

.footer .footer-container .credit span a{
    color:var(--orange);
}

.footer .footer-container .credit span a:hover{
    color:white;
    background-color: indigo;
    padding: 0px 5px;
}






















/* media queries  */

@media (max-width:991px){

    html{
        font-size: 55%;
    }

    header{
        padding:1.5rem;
    }

    section{
        padding:1.5rem;
    }

    .home .content h3{
        font-size: 5rem;
    }

}

@media (max-width:768px){

    header{
        flex-flow: column;
    }

    header form{
        width:100%;
        margin:2rem 0;
    }

    header.active{
        transform: translateY(-12.5rem);
    }

    .home .content{
        text-align: center;
    }

    .home .image img{
        width: 100%;
    }

}

@media (max-width:450px){

    html{
        font-size: 50%;
    }

    .heading{
        text-align: center;
        font-size: 2.5rem;
        border-bottom: none;
    }

}
    </style>

</head>
<body>
    
<!-- header section starts  -->

<header>

    <a href="#" class="logo"><img src="./img/logoo.jpg" height="70px"><span></span></a>

    <form action="">
        <input type="search" id="search-bar">
        <label for="search-bar" class="fas fa-search"></label>
    </form>

    <div class="icons">
        <div id="menu-bar" class="fas fa-bars"></div>
        <div id="theme-toggler" class="fas fa-moon"></div>
        <a href="#products" class="fas fa-heart"></a>
        <a href="http://wa.me/9940489085" target="_blank" class="fas fa-shopping-cart"></a>
        <a href="#logoo" class="fas fa-user"></a>
    </div>

</header>

<!-- header section ends -->

<!-- navbar section  -->

<nav class="navbar">

    <div class="user">
        <img src="./img/logoo.jpg" alt="">
        <h3>Banuja fashion home</h3>
    </div>

    <div class="links">
        <a href="#home">home</a>
        <a href="#products">products</a>
        <a href="#featured">featured</a>
        <a href="#deal">deal</a>
        <a href="#review">review</a>
    </div>

    <div id="close" class="fas fa-times"></div>

</nav>
<section class="home" id="home">

    <div class="content">
        <span>special offer</span>
        <h3>sale upto 50% off</h3>
        <h3>PATTERN WORK SPECALIST</h3>
        <a href="http://wa.me/+919940489085" target="_blank" class="btn">shop now</a>
    </div>

    <div class="image">
        <img src="./img/logo2.jpg" alt="">
    </div>

</section>

<!-- home section ends -->

<!-- category section starts  -->

<section class="category">

    <h1 class="heading"> shop by <span>category</span> </h1>

    <div class="box-container">

        <div class="box">
            <img src="img/a1.jpg" alt="">
            <div class="content">
                <span>upto 50% off</span>
                <h3>for womans</h3>
                <a href="http://wa.me/9940489085" target="_blank" class="btn">shop now</a>
            </div>
        </div>

        <div class="box">
            <img src="./img/pp2.jpg" alt="">
            <div class="content">
                <span>upto 50% off</span>
                <h3>PATTERN WORK SPEACALIST</h3>
                <a href="http://wa.me/+919940489085" target="_blank" class="btn">shop now</a>
            </div>
        </div>
        
    </div>

</section>
<!-- products section starts  -->

<section class="products" id="products">

    <h1 class="heading"> latest <span>products</span> </h1>

<div class="swiper-container product-slider gap">
    <div class="swiper-wrapper">
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="lehanga.jpg" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="lehanga.jpg" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>Lehanga Stitching</h3>
                    <div class="price">&#8377;900<span>&#8377;1500</span></div>
                    <a href="http://wa.me/+919940489085" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/max1.webp" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/max1.webp" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>Pleated maxi gown</h3>
                    <div class="price">&#8377;600<span>&#8377;1000</span></div>
                    <a href="http://wa.me/+919940489085" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/scc.jpg" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/scc.jpg" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>saree convert stitching</h3>
                    <div class="price">&#8377;800<span>&#8377;1000</span></div>
                    <a href="http://wa.me/+919940489085" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/um1.webp" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/um1.webp" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3> Umbrella maxi gown</h3>
                    <div class="price">&#8377;600<span>&#8377;800</span></div>
                    <a href="http://wa.me/+919940489085" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/part.webp" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/part.webp" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3> Part cutting maxi gown</h3>
                    <div class="price">&#8377;800<span>&#8377;1500</span></div>
                    <a href="http://wa.me/+919940489085" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/ga1.webp" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/ga1.webp" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>Gethering maxi gown</h3>
                    <div class="price">&#8377;600<span>&#8377;1000</span></div>
                    <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
    </div>
    <div class="swiper-button-next"></div>
    <div class="swiper-button-prev"></div>
</div>

<div class="swiper-container product-slider">
    <div class="swiper-wrapper">
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/normal.jpg" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/normal.jpg" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>Normal Blouse Stitching</h3>
                    <div class="price">&#8377;150<span>&#8377;200</span></div>
                    <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/l.jpg"  target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/l.jpg" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>Lining blouse stitching</h3>
                    <div class="price">&#8377;300 <span>&#8377;350</span></div>
                    <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/p.jpg" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/p.jpg" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>Pattern Blouse Stitching</h3>
                    <div class="price">&#8377;1000<span>&#8377;2000</span></div>
                    <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/pr1.jpg" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/pr1.jpg" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>Princess cutting</h3>
                    <div class="price">&#8377;300<span>&#8377;500</span></div>
                    <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
      
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/mom.jpg" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/mom.jpg" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>Combo Dress Stitching</h3>
                    <div class="price">&#8377; 700<span>&#8377;1000</span></div>
                    <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="icons">
                    <a href="#deal" class="fas fa-heart"></a>
                    <a href="#search-bar" class="fas fa-search"></a>
                    <a href="./img/ari.jpg" target="_blank" class="fas fa-eye"></a>
                </div>
                <div class="image">
                    <img src="./img/ari.jpg" alt="">
                </div>
                <div class="content">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="far fa-star"></i>
                        <span>( 250 reviews )</span>
                    </div>
                    <h3>Ari Blouse Design Starting</h3>
                    <div class="price">&#8377;1000<span>&#8377;7000</span></div>
                    <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
                </div>
            </div>
        </div>
        
    </div>
    <div class="swiper-button-next"></div>
    <div class="swiper-button-prev"></div>
</div>


</section>

<!-- products section ends -->

<!-- featured section starts  -->

<section class="featured" id="featured">

    <h1 class="heading"> <span>featured</span> products </h1>

    <div class="box-container">

        <div class="box">
            <div class="image-container">
                <div class="small-image">
                    <img src="./img/d1.jpg" class="small-image-1" alt="">
                    <img src="./img/d2.jpg" class="small-image-1" alt="">
                    <img src="./img/d3.jpg" class="small-image-1" alt="">
                </div>
                <div class="big-image">
                    <img src="./img/d1.jpg" class="big-image-1" alt="">
                </div>
            </div>
            <div class="content">
                <h3>Dhothi</h3>
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="far fa-star"></i>
                    <span>( 250 reviews )</span>
                </div>
                <p>Chaitanya is supplied uninterruptedly to the region below the waist, and the distressing energy there gets destroyed.</p>
                <div class="price">&#8377;500<span>&#8377;700</span></div>
                <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
            </div>
        </div>

        <div class="box">
            <div class="image-container">
                <div class="small-image">
                    <img src="./img/cig1.jpg" class="small-image-2" alt="">
                    <img src="./img/cig2.jpg" class="small-image-2" alt="">
                    <img src="./img/cig3.jpg" class="small-image-2" alt="">
                </div>
                <div class="big-image">
                    <img src="./img/cig1.jpg" class="big-image-2" alt="">
                </div>
            </div>
            <div class="content">
                <h3>Cigratte Pant</h3>
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="far fa-star"></i>
                    <span>( 250 reviews )</span>
                </div>
                <p>Cigarette shape is best for an athletic or hourglass body. </p>
                <div class="price">&#8377; 500<span>&#8377;700</span></div>
                <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
            </div>
        </div>

        <div class="box">
            <div class="image-container">
                <div class="small-image">
                    <img src="./img/patt1.jpg" class="small-image-3" alt="">
                    <img src="./img/patt2.jpg" class="small-image-3" alt="">
                    <img src="./img/patt3.jpg" class="small-image-3" alt="">
                </div>
                <div class="big-image">
                    <img src="./img/patt1.jpg" class="big-image-3" alt="">
                </div>
            </div>
            <div class="content">
                <h3> Pattiyala pant salwar set</h3>
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="far fa-star"></i>
                    <span>( 250 reviews )</span>
                </div>
                <p> a plain Salwar with a printed kurta with a heavy dupatta.</p>
                <div class="price">&#8377; 400<span>&#8377;600</span></div>
                <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
            </div>
        </div>
        
        <div class="box">
            <div class="image-container">
                <div class="small-image">
                    <img src="./img/new1.jpg" class="small-image-4" alt="">
                    <img src="./img/new2.jpg" class="small-image-4" alt="">
                    <img src="./img/new3.jpg" class="small-image-4" alt="">
                </div>
                <div class="big-image">
                    <img src="./img/new4.jpg" class="big-image-4" alt="">
                </div>
            </div>
            <div class="content">
                <h3>Ari work stitching</h3>
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="far fa-star"></i>
                    <span>( 250 reviews )</span>
                </div>
                <p> A pen like needle, that resembles a crochet needle is used to do the intrinsic Aari work..</p>
                <div class="price">&#8377; 1000<span>&#8377;5000</span></div>
                <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
            </div>
        </div>
        <div class="box">
            <div class="image-container">
                <div class="small-image">
                    <img src="./img/new5.webp" class="small-image-5" alt="">
                    <img src="./img/new6.webp" class="small-image-5" alt="">
                    <img src="./img/new7.webp" class="small-image-5" alt="">
                </div>
                <div class="big-image">
                    <img src="./img/new5.webp" class="big-image-5" alt="">
                </div>
            </div>
            <div class="content">
                <h3>Blouse Collection Creativity</h3>
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="far fa-star"></i>
                    <span>( 250 reviews )</span>
                </div>
                <p>Blouse designs are formed on the basis of texture of the fabric.</p>
                <div class="price">&#8377; 300<span>&#8377;1000</span></div>
                <a href="http://wa.me/+919944605621" target="_blank" class="btn">add to cart</a>
            </div>
        </div>


        


    </div>

</section>

<!-- featured section ends -->

<!-- deal section starts  -->

<section class="deal" id="deal">

    <h1 class="heading"> special <span>deal</span> </h1>

    <div class="row">

        <div class="content">
            <span class="discount">upto 50% off</span>
            <h3 class="text">deal of the day</h3>
            <div class="count-down">
                <div class="box">
                    <h3 id="days">00</h3>
                    <span>days</span>
                </div>
                <div class="box">
                    <h3 id="hours">00</h3>
                    <span>hours</span>
                </div>
                <div class="box">
                    <h3 id="minutes">00</h3>
                    <span>minutes</span>
                </div>
                <div class="box">
                    <h3 id="seconds">00</h3>
                    <span>seconds</span>
                </div>
            </div>
            <a href="http://wa.me/+919944605621" target="_blank" class="btn">shop now</a>
        </div>

        <div class="image">
            <img src="./img/counter.jpg" alt="">
        </div>

    </div>

</section>

<!-- deal section ends -->

<!-- review section starts  -->

<section class="review" id="review">

    <h1 class="heading"> customers <span>review</span> </h1>

<div class="swiper-container review-slider">
    <div class="swiper-wrapper">
        <div class="swiper-slide">
            <div class="slide">
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                </div>
                <p>stitching blouse
                    Thank you so much....i resived beautiful kurti..i can't believe I'm so happy
                    
                    Nice quality wise is very good and colour be very better
                    
                    Not cotton but fabric is very lightweight and good 😊. </p><br><br>
                <div class="user">
                    <img src="./img/m22.jpg" alt="">
                    <div class="user-info">
                        <h3>Malini</h3>
                        <span>happy customer</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                </div>
                <p>pattupavadai
                    Awesome product❤thank u
                    
                    its nice ,very good product ,must buy it 👍🏻👌🏻👏🏻👏🏻👏🏻😍🤩
                    
                    Really good the fabric is nice must buy it I love ❤️❤️❤️❤️❤️❤️❤️
                    
                    Looking good... Worth for cost..
                    Clothes is very good I received XL it's good product 👍</p>
                <div class="user">
                    <img src="./img/pr3.jpg" alt="">
                    <div class="user-info">
                        <h3>Saravanan</h3>
                        <span>happy customer</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                </div>
                <p>Worth the money 🤑💰
                    
                    Excellent product thanku.Product was great...just as shown in picture...just dissappointed with the quality of the product 
                    but then its worth in the price
                    Clothes is very good I received XL it's good product 👍</p>
                <div class="user">
                    <img src="./img/pr2.jpg" alt="">
                    <div class="user-info">
                        <h3>Malik</h3>
                        <span>happy customer</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="swiper-slide">
            <div class="slide">
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                </div>
                <p>Pattern Blouse
                    Happy with the product according to the price. True to size
                    
                    Excellent soo smooth super tq so much
                    
                    Good value money product
                    
                    Very good quality I love it 😇😇.
                    Very nice dress and quality is also good and I like it very much and thank you</p>
                <div class="user">
                    <img src="./img/pr4.jpg" alt="">
                    <div class="user-info">
                        <h3>Kalima</h3>
                        <span>happy customer</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

</section>

<!-- review section ends -->

<!-- footer section starts  -->

<section class="footer">

<div class="footer-container">

    <div class="box-container">

        <div class="box">
            <h3>quick links</h3>
            <a href="#">home</a>
            <a href="#">products</a>
            <a href="#">featured</a>
            <a href="#">deal</a>
            <a href="#">review</a>
        </div>

        <div class="box">
            <h3>extra links</h3>
            <a href="#">my account</a>
            <a href="#">my favorite</a>
            <a href="#">my order</a>
            <a href="#">my cart</a>
        </div>

        

        <div class="box">
            <h3> Social links</h3>
            <a href="https://instagram.com/banuja_creation_22?igshid=OGQ5ZDc2ODk2ZA==" target="_blank"> <i class="fab fa-instagram"></i> instagram</a>
            <a href="http://wa.me/+919944605621" target="_blank"> <i class="fab fa-whatsapp"></i> Whats app</a>
        </div>

        <div class="box">
            <h3>contact us</h3>
            <a href="http://wa.me/+919944605621" target="_blank">+91 9944605621</a>
            <a href="#">redbutterfly1092@gmail.com</a>
            <a href="#">257 SKP Street Tenkasi - 627811</a>
            <h3>payment methods</h3>
            <img src="./img/payment.png" alt="Payment Image">
        </div>

    </div>

    <div class="credit"> created by <span> <a href="https://instagram.com/web_developer_vf?igshid=OGQ5ZDc2ODk2ZA=="> VF WEBDESIGNER </a> </span> | all rights reserved </div>

</div>

</section>

<!-- footer section ends -->
















<script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>


<!-- category section ends -->
<script src="script.js"></script>
<script>
    let navbar = document.querySelector('.navbar')

document.querySelector('#menu-bar').onclick = () =>{
    navbar.classList.toggle('active');
}

document.querySelector('#close').onclick = () =>{
    navbar.classList.remove('active');
}

window.onscroll = () =>{

    navbar.classList.remove('active');

    if(window.scrollY > 100){
        document.querySelector('header').classList.add('active');
    }else{
        document.querySelector('header').classList.remove('active');
    }

}

let themeToggler = document.querySelector('#theme-toggler');

themeToggler.onclick = () =>{
    themeToggler.classList.toggle('fa-sun');
    if(themeToggler.classList.contains('fa-sun')){
        document.querySelector('body').classList.add('active');
    }else{
        document.querySelector('body').classList.remove('active');
    }
}

document.querySelectorAll('.small-image-1').forEach(images =>{
    images.onclick = () =>{
        document.querySelector('.big-image-1').src = images.getAttribute('src');
    }
});

document.querySelectorAll('.small-image-2').forEach(images =>{
    images.onclick = () =>{
        document.querySelector('.big-image-2').src = images.getAttribute('src');
    }
});

document.querySelectorAll('.small-image-3').forEach(images =>{
    images.onclick = () =>{
        document.querySelector('.big-image-3').src = images.getAttribute('src');
    }
});
document.querySelectorAll('.small-image-4').forEach(images =>{
    images.onclick = () =>{
        document.querySelector('.big-image-4').src = images.getAttribute('src');
    }
});
document.querySelectorAll('.small-image-5').forEach(images =>{
    images.onclick = () =>{
        document.querySelector('.big-image-5').src = images.getAttribute('src');
    }
});




let countDate = new Date('aug 1, 2021 00:00:00').getTime();

function countDown(){

    let now = new Date().getTime();
	gap = countDate - now;

    let seconds = 1000;
    let minutes = seconds * 60;
    let hours = minutes * 60;
    let days = hours * 24;

    let d = Math.floor(gap / (days));
	let h = Math.floor((gap % (days)) / (hours));
	let m = Math.floor((gap % (hours)) / (minutes));
	let s = Math.floor((gap % (minutes)) / (seconds));

    document.getElementById('days').innerText = d;
    document.getElementById('hours').innerText = h;
    document.getElementById('minutes').innerText = m;
    document.getElementById('seconds').innerText = s;

}

setInterval(function(){
    countDown()
},1000);

var swiper = new Swiper(".product-slider", {
    slidesPerView: 3,
    loop:true,
    spaceBetween: 10,
    autoplay: {
        delay: 4000,
        disableOnInteraction: false,
    },
    navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev",
    },
    breakpoints: {
        0: {
            slidesPerView: 1,
        },
        550: {
          slidesPerView: 2,
        },
        800: {
          slidesPerView: 3,
        },
        1000: {
            slidesPerView: 3,
        },
    },
});

var swiper = new Swiper(".review-slider", {
    slidesPerView: 3,
    loop:true,
    spaceBetween: 10,
    autoplay: {
        delay: 4000,
        disableOnInteraction: false,
    },
    breakpoints: {
        0: {
            slidesPerView: 1,
        },
        550: {
          slidesPerView: 2,
        },
        800: {
          slidesPerView: 3,
        },
        1000: {
            slidesPerView: 3,
        },
    },
});
</script>
</body></html>
