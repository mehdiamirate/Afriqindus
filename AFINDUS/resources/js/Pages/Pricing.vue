<template>
    <div><section>
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

          <h1>
              A Plan For Every Price, choose your plan
          </h1>

          <div class="pricing-cards">
              <div class="pricing-card">
                  <p class="plan">Starter</p>
                  <p class="description">
                    The basics for personal projects, hobby sites, or experiments.
                  </p>

                  <a href="./contact.html"> GET STARTED </a>

                  <div class="price">
                      $ <span>per month</span>
                  </div>

                  <ul>
                    <li>Lorem ipsum dolor sit amet consectetur.</li>
                    <li>Lorem ipsum dolor sit amet.</li>
                    <li>Lorem ipsum dolor sit amet conse.</li>
                    <li>Lorem ipsum dolor sit amet consec tetur.</li>
                    <li>Lorem ipsum dolor sit amet cons ecte tur.</li>
                    <li>Lorem ipsum dolor sit amet consectetur.</li>
                  </ul>
              </div>

              <div class="pricing-card">
                <p class="plan">Pro</p>
                <p class="description">
                  Advanced features and support for building pilot projects or small
                  sites.
                </p>
      
                <a href="./contact.html"> GET STARTED </a>
      
                <div class="price">$ <span>per month</span></div>
      
                <ul>
                  <li>Everything from free plan.</li>
                  <li>Lorem ipsum dolor sit amet.</li>
                  <li>Lorem ipsum dolor sit amet conse.</li>
                  <li>Lorem ipsum dolor sit amet consec tetur.</li>
                  <li>Lorem ipsum dolor sit amet cons ecte tur.</li>
                  <li>Lorem ipsum dolor sit amet consectetur.</li>
                </ul>
              </div>
      
              <div class="pricing-card">
                <p class="plan">Enterprise</p>
                <p class="description">
                  Collaboration, security, & compliance for scaling web apps and dev
                  teams.
                </p>
      
                <a href="./contact.html"> GET STARTED </a>
      
                <div class="price">$ <span>per month</span></div>
      
                <ul>
                  <li>Pro features, plus:</li>
                  <li>Lorem ipsum dolor sit amet.</li>
                  <li>Lorem ipsum dolor sit amet conse.</li>
                  <li>Lorem ipsum dolor sit amet consec tetur.</li>
                  <li>Lorem ipsum dolor sit amet cons ecte tur.</li>
                  <li>Lorem ipsum dolor sit amet consectetur.</li>
                </ul>
              </div>
          </div>
    </section>

    <div class="copyright">&copy; Afriqindus</div>
    </div>
</template>

<style>
section{
    background:  linear-gradient(rgba(255,255,255,.5), rgba(255,255,255,.5)), url(""); /* no repeat to avoid multi the pic in a big screen */
    background-size: cover;
    min-height: 100vh;
    background-color: rgb(21,76,121);
}

section > h1{
    color: #fff;
    text-align: center;
    margin: 1rem 0;
    font-size: 2.5rem;
}

.pricing-cards{
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    padding: 2rem;
}

.pricing-card{
    background-color: #fff;
    border-radius: 10px;
    text-align: center;
    margin:1rem;
    width: 275px;
    min-height: 400px;
    padding: 1rem .75rem;
    box-shadow:1px 2px 10px 1px #333;
}

.pricing-card .plan{
    font-size: 2rem;
}

.pricing-card .description{
    font-size: .9rem;
    margin-top: .5rem;
    margin-bottom: 1rem;
}

.pricing-card > a{
    background-color: royalblue;
    text-decoration: none;
    color: #fff;
    padding: 10px 25px;
    border-radius: 5px;
    transition: .3s ease-in-out;
}

.pricing-card > a:hover{
    background-color: rgb(31, 60, 150);
}

.pricing-card .price{
    font-weight: bold;
    font-size: 2rem;
    padding: 10px 0;
    margin-top:1.5rem;
}

.pricing-card .price span{
    font-size: 1rem;
}

.pricing-card ul{
    text-align: left;
    padding: 0 1rem;
}

.pricing-card ul li{
    font-size: .9rem;
    list-style-type: circle;
    padding-top: 5px;
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
</style>