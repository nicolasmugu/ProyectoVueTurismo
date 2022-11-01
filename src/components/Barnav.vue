<template>
<header class="header" id="header">
    <nav class="nav container">
         <div class="logo">
                    <a href="#" class="nav__logo"><img src="./../assets/img/logo.png" alt="logo" class="logo1" ></a> 
                    <a href="#" class="nav__logo-1"><img src="./../assets/img/logo1.png" alt="logo"  class="logo1"></a>
                </div>
        <div class="nav__menu" id="nav-menu">
            <ul class="nav__list">
                <li class="nav__item">
                    <a href="#home" class="nav__link active-link">Inicio</a>
                </li>
                <li class="nav__item">
                    <a href="#about" class="nav__link">Informaci&oacute;n</a>
                </li>
                <li class="nav__item">
                    <a href="#place" class="nav__link">Lugares</a>
                </li>
                <li class="nav__item">
                    <a href="#hotel" class="nav__link">Hoteles</a>
                </li>
                <li class="nav__item">
                    <a href="#login" class="nav__link">Login</a>
                </li>
                <li class="nav__item">
                    <a href="#login" class="nav__link">Registre</a>
                </li>
            </ul>
<!-- Mauricio-->
            <i class="ri-close-line nav__close" id="nav-close"></i>
        </div>

        <div class="nav__toggle" id="nav-toggle">
            <i class="ri-function-line"></i>
        </div>
    </nav>
</header>
</template>
<style>
/*========== Button Dark/Light ==========*/
/*=============== GOOGLE FONTS ===============*/
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&family=Raleway:wght@500;600;700&display=swap");

/*=============== VARIABLES CSS ===============*/
:root {
  --header-height: 3rem;

  /*========== Colors ==========*/
  /* Change favorite color to match images */
  /*Green dark 190 - Green 171 - Grren Blue 200*/
  --hue-color: 200;

  /* HSL color mode */
  --first-color: hsl(var(--hue-color), 64%, 22%);
  --first-color-second: hsl(var(--hue-color), 64%, 22%);
  --first-color-alt: hsl(var(--hue-color), 64%, 15%);
  --title-color: hsl(var(--hue-color), 64%, 18%);
  --text-color: hsl(var(--hue-color), 24%, 35%);
  --text-color-light: hsl(var(--hue-color), 8%, 60%);
  --input-color: hsl(var(--hue-color), 24%, 97%);
  --body-color: hsl(var(--hue-color), 100%, 99%);
  --white-color: #FFF;
  --scroll-bar-color: hsl(var(--hue-color), 12%, 90%);
  --scroll-thumb-color: hsl(var(--hue-color), 12%, 75%);

  /*========== Font and typography ==========*/
  --body-font: 'Open Sans', sans-serif;
  --title-font: 'Raleway', sans-serif;
  --biggest-font-size: 2.5rem;
  --h1-font-size: 1.5rem;
  --h2-font-size: 1.25rem;
  --h3-font-size: 1rem;
  --normal-font-size: .938rem;
  --small-font-size: .813rem;
  --smaller-font-size: .75rem;

  /*========== Font weight ==========*/
  --font-medium: 500;
  --font-semi-bold: 600;

  /*========== Margenes Bottom ==========*/
  --mb-0-25: .25rem;
  --mb-0-5: .5rem;
  --mb-0-75: .75rem;
  --mb-1: 1rem;
  --mb-1-25: 1.25rem;
  --mb-1-5: 1.5rem;
  --mb-2: 2rem;
  --mb-2-5: 2.5rem;

  /*========== z index ==========*/
  --z-tooltip: 10;
  --z-fixed: 100;

  /*========== Hover overlay ==========*/
  --img-transition: .3s;
  --img-hidden: hidden;
  --img-scale: scale(1.1);
}

@media screen and (min-width: 968px) {
  :root {
    --biggest-font-size: 4rem;
    --h1-font-size: 2.25rem;
    --h2-font-size: 1.75rem;
    --h3-font-size: 1.25rem;
    --normal-font-size: 1rem;
    --small-font-size: .875rem;
    --smaller-font-size: .813rem;
  }
}
/*=============== BASE ===============*/
* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}

html {
    scroll-behavior: smooth;
}

body {
    margin: var(--header-height) 0 0 0;
    font-family: var(--body-font);
    font-size: var(--normal-font-size);
    background-color: var(--body-color)  ;
    color: var(--text-color);
}

h1, h2, h3 {
    color: var(--title-color);
    font-weight: var(--font-semi-bold);
    font-family: var(--title-font);
}

ul {
    list-style: none;
}

a {
    text-decoration: none;
}

img {
    max-width: 100%;
    height: auto;
}

button,
input {
    border: none;
    font-family: var(--body-font);
    font-size: var(--normal-font-size);
}

button {
    cursor: pointer;
}

input {
    outline: none;
}

.nav__dark {
  display: flex;
  align-items: center;
  column-gap: 2rem;
  position: absolute;
  left: 3rem;
  bottom: 4rem;
}

.change-theme, .change-theme-name {
  color: var(--text-color);
}

.change-theme {
  cursor: pointer;
  font-size: 1rem;
}

.change-theme-name {
  font-size: var(--small-font-size);
}

/*=============== REUSABLE CSS CLASSES ===============*/
.container {
  max-width: 968px;
  margin-left: var(--mb-1);
  margin-right: var(--mb-1);
}

/*=============== HEADER ===============*/
.header {
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  z-index: var(--z-fixed);
  background-color: transparent;
}

/*=============== NAV ===============*/
.nav{
  height: var(--header-height);
  display: flex;
  justify-content: space-between;
  align-items:center;
}

.logo{
  height: 10rem;
  display: flex;
}
.nav__toggle {
  color: var(--white-color);
}

.nav__logo {
  position:absolute;
  visibility: visible;
}
.logo1{
  flex: auto;
  width: 100px;
  height: 55px;
  margin-top: 50px;
}

@media (min-width: 770px) {
    .logo1{
      width: 130px;
      height: 70px;
      margin-top: 40px;
    }
}
    .nav__logo-1{
    position: absolute;
    visibility: hidden;
    }
    .nav__toggle {
    font-size: 1.2rem;
    cursor: pointer;
    }

    .nav__menu {
    position: relative;
    }

@media screen and (max-width: 767px) {
  .nav__menu {
    position: fixed;
    background-color: var(--body-color);
    top: 0;
    right: -100%;
    width: 70%;
    height: 100%;
    box-shadow: -1px 0 4px rgba(14, 55, 63, 0.15);
    padding: 3rem;
    transition: .4s;
  }

}

.nav__list {
    display: flex;
    flex-direction: column;
    row-gap: 2.5rem;
}

.nav__link {
  color: var(--text-color-light);
  font-weight: var(--font-semi-bold);
  text-transform: uppercase;
}

.nav__link:hover {
  color: var(--text-color);
}

.nav__close {
  position: absolute;
  top: .75rem;
  right: 1rem;
  font-size: 1.5rem;
  color: var(--title-color);
  cursor: pointer;
}

/* show menu */
.show-menu {
  right: 0;
}

/* Change background header */
.scroll-header {
  background-color: var(--body-color);
  box-shadow: 0 0 4px rgba(14, 55, 63, 0.15);
}

.scroll-header .nav__logo{
    visibility: hidden;
}
.scroll-header .nav__logo-1 {
  visibility: visible;
}
.scroll-header .nav__toggle {
  color: var(--title-color);
}

/* Active link */
.active-link {
  position: relative;
  color: var(--title-color);
}

.active-link::before {
  content: '';
  position: absolute;
  background-color: var(--title-color);
  width: 100%;
  height: 2px;
  bottom: -.75rem;
  left: 0;
}
@media screen and (min-width: 768px) {
    .nav {
        height: calc(var(--header-height) + 1.5rem);
    }
    .nav__link {
        color: var(--white-color);
        text-transform: initial;
    }
    .nav__link:hover {
        color: var(--white-color);
    }
    .nav__dark {
        position: initial;
    }
    .nav__menu {
        display: flex;
        column-gap: 1rem;
    }
    .nav__list {
        flex-direction: row;
        column-gap: 4rem;
    }
    .nav__toggle, .nav__close {
        display: none;
    }
    .change-theme-name {
        display: none;
    }
    .change-theme {
        color: var(--white-color);
    }
    .active-link::before {
        background-color: var(--white-color);
    }
    .scroll-header .nav__link {
        color: var(--text-color);
    }
    .scroll-header .active-link {
        color: var(--title-color);
    }
    .scroll-header .active-link::before {
        background-color: var(--title-color);
    }
    .scroll-header .change-theme {
        color: var(--text-color);
    }
}
@media screen and (min-width: 1024px) {
    .container {
            margin-left: auto;
            margin-right: auto;
        }
}
@media screen and (min-width: 1200px) {
    .container {
        max-width: 1024px;
    }
}

</style>
