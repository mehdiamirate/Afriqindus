<template>
    <div>
        <section class="contact-main">
      <nav>
        <div class="brand">
          
          <a href="/">Afriqindus</a>
        </div>

        <i class="fa fa-bars" aria-hidden="true"></i>

        <ul>
          <i class="fa fa-times" aria-hidden="true"></i>
          <li><a href="/">Home</a></li>
          <li><a href="Pricing">Pricing</a></li>
          <li><a href="Contact">Contact</a></li>
          <li><a href="./login.html">Sign in</a></li>
        </ul>
      </nav>

      <div class="contact-main-text">
        <h1>Our teams are here to help</h1>
        <p>
          Get in touch and let us know how we can help. We’ll help you combine
          the flexibility of the digital solutions with the control and compliance your
          business needs.
        </p>
        <a href="#contact">Need help?</a>
      </div>
    </section>

    <section class="contact-form" id="contact">
      <h1>Contact our team directly</h1>
      <form action="https://formsubmit.co/3c8b0efbdd8eccc2a6cbbbf3edbfd0a6 " method="POST">
        <input type="text" name="fname" placeholder="First name" required />
        <input type="text" name="lname" placeholder="Last name" required />
        <input type="email" name="email" placeholder="Email address" required />
        <input type="text" name="phone" placeholder="Phone" required />
        <input
          type="text"
          name="company"
          placeholder="Company/organization"
          required
        />
        <textarea
          name="query"
          id=""
          cols="30"
          rows="5"
          placeholder="Project details or questions"
        ></textarea>

        <button type="submit">Submit</button>
      </form>

      <div class="social-medias">
        <h3>& contact us on social media</h3>
        <ul>
          <li><a href="#"><i class="fa fa-facebook"></i>Facebook</a></li>
          <li><a href="#"><i class="fa fa-twitter"></i>Twitter</a></li>
          <li><a href="#"><i class="fa fa-instagram"></i>Instagram</a></li>
          <li><a href="#"><i class="fa fa-youtube"></i>YouTube</a></li>
          <li><a href="#"><i class="fa fa-linkedin"></i>Linkedin</a></li>
          <li><a href="mailto:contact@aashish-panthi.com.np"><i class="fa fa-envelope"></i>Email</a></li>
        </ul>
      </div>
    </section>
    <div class="copyright">&copy; Afriqindus</div>

    
    </div>
</template>

<style>
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

.contact-main {
    background:  linear-gradient(rgba(255,255,255,.5), rgba(255,255,255,.5)), url(""); /* no repeat to avoid multi the pic in a big screen */
    color: #fff;
  min-height: 100vh;
  background-color: rgb(21,76,121);
}

.contact-main-text{
    position: absolute;
    top:50%;
    left:50%;
    transform: translate(-50%,-50%);
    padding: 1rem;
    min-width: 75%;
    text-align: center;
}

.contact-main-text h1{
    font-size: 4rem;
}

.contact-main-text p{
    font-size: 1.5rem;
    margin: 1rem 0 2rem 0;
}

.contact-main-text a{
    text-decoration: none;
    color: #fff;
    padding: 10px 25px;
    border: 1px solid #fff;
    position: relative;
}

.contact-main-text a::before{
    content: '';
    position: absolute;
    top:0;
    left: 0;
    background-color: chocolate;
    width: 100%;
    height: 100%;
    z-index: -1;
    transform: scaleX(0);
    transition: .2s ease-in-out;
}

.contact-main-text a:hover::before{
    transform: scaleX(1);
}

@media screen and (max-width: 600px) {
    .contact-main-text{
        width: 90%;
    }

    .contact-main-text h1{
        font-size: 2rem;
    }

    .contact-main-text p{
        font-size: 1rem;
    }
}

.contact-form{
    text-align: center;
    padding: 1rem;
}

.contact-form form{
    max-width: 500px;
    margin:2rem auto;
    display: flex;
    flex-direction: column;
}

.contact-form form input{
    height: 40px;
    padding: 5px 10px;
    outline: none;
    margin-bottom: 5px;
}

.contact-form form textarea{
    padding: 5px 10px;
    outline: none;
}

.contact-form form input:focus, .contact-form form textarea:focus{
    outline: 1px solid royalblue;
}

.contact-form form button{
    background-color: royalblue;
    height: 40px;
    color: #fff;
    border-radius: 5px;
    cursor: pointer;
    border: none;
    margin:5px 0;
    transition: .3s ease-in-out;
}

.contact-form form button:hover{
    background-color: rgb(35, 64, 150);
}

.social-medias{
    max-width: 500px;
    margin:0 auto;
    text-align: left;
}

.social-medias ul li{
    list-style: none;
}

.social-medias ul li a{
    text-decoration: none;
    color: #555;
}

.social-medias ul li a:hover{
    color: #000;
}

.social-medias ul li a i{
    color: #000;
    margin-right: 5px;
}

.social-medias ul li a:hover i{
    color: rgb(70, 41, 173);
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