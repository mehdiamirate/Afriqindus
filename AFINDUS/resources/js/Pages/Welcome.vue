

<template>


    
    <section class="home-main">
        <nav>
            <div class="brand">
               
                <!-- logo top left -->
                <a href="index.html">Afriqindus</a>
            </div>

            <i class="fa fa-bars" aria-hidden="true"></i>

            <ul>
                <i class="fa fa-times" aria-hidden="true"></i>
                <li><a href="">Home</a></li>
                <li><a href="Pricing">Pricing</a></li>
                <li><a href="Contact">Contact</a></li>
                <li><a href="./login.html">Sign in</a></li>
            </ul>
        </nav>

        <div class="main-content">
            <h1>slogant</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut atque repellendus tempore magnam nihil quibusdam beatae quod ipsum molestias? Doloribus esse culpa, sit nisi recusandae facere deleniti ducimus asperiores! Inventore? Ut aut deleniti
                distinctio labore nisi possimus voluptatem dolores modi doloribus expedita at qui esse necessitatibus provident sapiente praesentium.</p>

            <a href="./contact.html" class="gradient-btn">CONTACT US</a>
        </div>
    </section>

    <section class="about">

        <div class="about-sub">
            
            <div class="sub-sub-about">
                <h2>About Us</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut atque repellendus tempore magnam nihil quibusdam beatae quod ipsum molestias? Doloribus esse culpa, sit nisi recusandae facere deleniti ducimus asperiores! Inventore? Ut aut deleniti distinctio
                    labore nisi possimus voluptatem dolores modi doloribus expedita at qui esse necessitatibus provident sapiente praesentium.
                </p>
                <a href="./login.html" class="gradient-btn">Get started</a>
            </div>
        </div>

        <div class="about-sub">
            <div class="sub-sub-about">
                <h2>Our Services </h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut atque repellendus tempore magnam nihil quibusdam beatae quod ipsum molestias? Doloribus esse culpa, sit nisi recusandae facere deleniti ducimus asperiores! Inventore? Ut aut deleniti distinctio
                    labore nisi possimus voluptatem dolores modi doloribus expedita at qui esse necessitatibus provident sapiente praesentium.
                </p>
                <a href="./login.html" class="gradient-btn">CONTACT US</a>
            </div>
            
        </div>
    </section>

    <div class="subscribe">
        <h2>Stay up to date with all Afriqindus offers & news</h2>
        <form action="https://formsubmit.co/3c8b0efbdd8eccc2a6cbbbf3edbfd0a6 " method="POST" class="subscribe-box">
            <input required type="email" name="subscription_email" placeholder="Enter your email address" />
            <button>Subscribe</button>
        </form>
    </div>

    <div class="copyright">&copy; Afriqindus</div>

    
    
    
</template>



<style scoped>
    .bg-gray-100 {
        background-color: #f7fafc;
        background-color: rgba(247, 250, 252, var(--tw-bg-opacity));
    }

    .border-gray-200 {
        border-color: #edf2f7;
        border-color: rgba(237, 242, 247, var(--tw-border-opacity));
    }

    .text-gray-400 {
        color: #cbd5e0;
        color: rgba(203, 213, 224, var(--tw-text-opacity));
    }

    .text-gray-500 {
        color: #a0aec0;
        color: rgba(160, 174, 192, var(--tw-text-opacity));
    }

    .text-gray-600 {
        color: #718096;
        color: rgba(113, 128, 150, var(--tw-text-opacity));
    }

    .text-gray-700 {
        color: #4a5568;
        color: rgba(74, 85, 104, var(--tw-text-opacity));
    }

    .text-gray-900 {
        color: #1a202c;
        color: rgba(26, 32, 44, var(--tw-text-opacity));
    }

    @media (prefers-color-scheme: dark) {
        .dark\:bg-gray-800 {
            background-color: #2d3748;
            background-color: rgba(45, 55, 72, var(--tw-bg-opacity));
        }

        .dark\:bg-gray-900 {
            background-color: #1a202c;
            background-color: rgba(26, 32, 44, var(--tw-bg-opacity));
        }

        .dark\:border-gray-700 {
            border-color: #4a5568;
            border-color: rgba(74, 85, 104, var(--tw-border-opacity));
        }

        .dark\:text-white {
            color: #fff;
            color: rgba(255, 255, 255, var(--tw-text-opacity));
        }

        .dark\:text-gray-400 {
            color: #cbd5e0;
            color: rgba(203, 213, 224, var(--tw-text-opacity));
        }
    }
    nav{
    height: 70px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 1rem;
}

nav .brand{
    display: flex;
    align-items: center;
}

nav .brand img{
    height: 50px;
    margin: 0 5px;
}

nav .brand a{
    color: rgb(239,247,247);
    text-decoration: none;
    font-size: 2rem;
    font-weight: bold;
}

nav ul{
    display: flex;
}

nav ul li{
    list-style: none;
    margin: 0 10px;
}

nav ul li a{
    text-decoration: none;
    color: #eff7f7;
    padding: 5px;
    transition: .3s ease;
    position: relative;
    font-size: 1.5rem;
}

nav ul li a:hover{
    color: #fff;
}

nav ul li a::after{
    content: '';
    width: 100%;
    height: 3px;
    background: rgb(255, 255, 255);
    position: absolute;
    bottom: 0;
    left:0;
    transform: scaleX(0);
    transform-origin: left;
    transition: .3s ease-in-out;
}

nav ul li a:hover::after{
    transform: scaleX(1);
}

nav .fa{
    color: rgb(29,75,154);
    font-size: 2rem;
    display: none;
}

@media screen and (max-width:600px) {

    nav .fa{
        display: block;
    }

    nav ul .fa{
        margin-bottom: 30px;
    }

    nav .brand img{
        height: 40px;
    }

    nav .brand a{
        font-size: 1.5rem;
    }
    nav ul{
        flex-direction: column;
        position: absolute;
        top:0;
        right:0;
        width:35%;
        background-color: rgb(36,149,226);
        padding:10px;
        height: 100vh;
        z-index: 99;
        transform: scaleX(0);
        transition: .1s ease-in;
        transform-origin: right;
    }
    
    nav ul.menu{
        transform: scaleX(1);
    }

    nav ul li {
        margin-top:10px;
    }

    nav ul li a{
        font-size: 1.25rem;
        font-weight: bold;
    }
}
*{
    margin:0;
    padding:0;
    box-sizing: border-box;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif; /* if the font is unavailable it moves to the next one */ 
    scroll-behavior: smooth;
}

body{
    min-height: 100vh;
}

.copyright{
    text-align: center;
    background-color: #eee;
    padding: 10px;
    font-size: .75rem;
}
.home-main {
  background:  linear-gradient(rgba(255,255,255,.5), rgba(255,255,255,.5)), url(""); /* no repeat to avoid multi the pic in a big screen */
  background-size: cover;
  min-height: 100vh;
  background-color: rgb(21,76,121);
}

.main-content {
  color: #fff;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 75%;
}

.main-content h1 { /*slogant*/
  font-size: 3rem;
}

.main-content p { /*paragraphe*/
  font-size: 1.2rem;
  margin: 0.5rem 0;
}

.gradient-btn {
  display: grid;
  place-items: center;
  text-decoration: none;
  color: #fff;
  background-image: linear-gradient(
    to right,
    rgb(36,149,226) 0%,
    rgb(29,75,154) 51%,
    rgb(36,149,226) 100%
  );
  border-radius: 10px;
  background-size: 200% auto;
  transition: 0.3s ease-in-out;
}

.main-content .gradient-btn {
  width: 200px;
  height: 45px;
  margin-top: 1.5rem;
  text-transform: uppercase;
}

.gradient-btn:hover {
  background-position: right center;
}

@media screen and (max-width: 600px) {
  .main-content h1 {
    font-size: 2.25rem;
  }

  .main-content p {
    font-size: 1rem;
  }

  .gradient-btn {
    width: 175px;
    height: 40px;
    font-size: 0.8rem;
  }
}

.about {
  padding: 1rem;
  text-align: center;
}

.about > h1 {
  font-size: 3rem;
  margin: 1rem 0;
}

.about-sub {
  display: flex;
  max-width: 800px;
  margin: 1rem auto;
  text-align: left;
}

.about-sub > img {
  max-height: 250px;
  width: 300px;
  max-width: 90%;
  animation: animateimage 1s linear;
}

@keyframes animateimage {
  from {
    transform: translateY(-15px);
    opacity: 0.5;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}

.about-sub .sub-sub-about {
  padding: 1rem;
  animation: animatetext 0.5s linear;
}

@keyframes animatetext {
  from {
    transform: translateY(15px);
    opacity: 0.5;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}

.about-sub .sub-sub-about p {
  font-size: 14px;
}

.about-sub .gradient-btn {
  width: 100px;
  margin-top: 5px;
  height: 30px;
  font-size: 12px;
}

@media screen and (max-width: 600px) {
  .about-sub {
    flex-direction: column;
  }

  .about-sub:nth-child(3) {
    flex-direction: column-reverse;
  }
}

.about-companies{
    max-width: 800px;
    width: 90%;
    background-color: #f1f1f1;
    padding: 1rem .5rem;
    margin:1rem auto;
}

.about-companies h1{
    font-size: 2rem;
    color: #444;
    text-transform: uppercase;
    margin-bottom: 1rem;
}

.about-companies h1 span{
    color: #000;
}

.about-companies .company-logos{
    display: flex;
    justify-content: space-evenly;
    color: #666;
    font-size: 2rem;
    transition: .3s ease-in;
    max-width: 75%;
    margin: 0pc auto;
}

.about-companies .company-logos .fa:hover{
    color: #000;
}

@media screen and (max-width:750px) {
    .about-companies h1{
        font-size: 1.5rem;
    }
}

@media screen and (max-width:600px) {
    .about-companies h1{
        font-size: 1.2rem;
    }

    .about-companies .company-logos{
        font-size: 1rem;
    }
}

.subscribe{
    text-align: center;
    padding: 3rem 2rem 2rem 2rem;
}

.subscribe-box{
    padding: 10px;
}

.subscribe-box input{
    max-width: 300px;
    width: 65%;
    padding: 5px 10px;
    height: 40px;
}

.subscribe-box button{
    border: none;
    background-color: #0072ff;
    height: 40px;
    padding: 0 1rem;
    color: #fff;
}
</style>
<script setup>
import { Head, Link } from '@inertiajs/inertia-vue3';

defineProps({
    canLogin: Boolean,
    canRegister: Boolean,
    laravelVersion: String,
    phpVersion: String,
});


</script>