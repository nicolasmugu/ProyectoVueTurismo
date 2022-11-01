<template>
<section class="about section" id="about">
    <div class="about__container container grid">
        <div class="about__data">
            <h2 class="section__title about__title">Más información <br> Sobre los mejores lugares</h2>
            <p class="about__description">Podrás encontrar los lugares, hoteles y tours más hermosos y agradables a los mejores
                precios con descuentos especiales, tu solo eliges el lugar y te guiaremos por todo el camino.
                <br> Consigue tu lugar ahora!
            </p>
            <a href="#" class="button">Reserva un lugar</a>
        </div>

        <div class="about__img">
            <div class="about__img-overlay">
                <img src="./../assets/img/about1.jpg" alt="" class="about__img-one">
            </div>

            <div class="about__img-overlay1">
                <img src="./../assets/img/about2.jpg" alt="" class="about__img-two">
            </div>
        </div>
    </div>
</section>
</template>
<style>
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

/*========== Variables Dark theme ==========*/
body.dark-theme {
    --first-color-second: hsl(var(--hue-color), 54%, 12%);
    --title-color: hsl(var(--hue-color), 24%, 95%);
    --text-color: hsl(var(--hue-color), 8%, 75%);
    --input-color: hsl(var(--hue-color), 29%, 16%);
    --body-color: hsl(var(--hue-color), 29%, 12%);
    --scroll-bar-color: hsl(var(--hue-color), 12%, 48%);
    --scroll-thumb-color: hsl(var(--hue-color), 12%, 36%);
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

.main {
  overflow-x: hidden;
}

/*=============== REUSABLE CSS CLASSES ===============*/
.section {
  padding: 4.5rem 0 2.5rem;
}

.section__title {
  font-size: var(--h2-font-size);
  color: var(--title-color);
  text-align: center;
  text-transform: capitalize;
  margin-bottom: var(--mb-2);
}

.container {
  max-width: 968px;
  margin-left: var(--mb-1);
  margin-right: var(--mb-1);
}

.grid {
  display: grid;
  gap: 1.5rem;
}

.button:active{
    transform: scale(0.7);
    transition: 0.4s;
    box-shadow: 0rem 0rem 20rem 0rem rgb(0, 255, 255);
}

    /*=============== ABOUT ===============*/
.about__data {
    text-align: center;
}

.about__container {
    row-gap: 2.5rem;
}

.about__description {
    margin-bottom: var(--mb-2);
}

.about__img {
    display: flex;
    column-gap: 1rem;
    align-items: center;
    justify-content: center;
}

.about__img-overlay {
    border-radius: 5px;
    height: 320px;
    overflow:var(--img-hidden);
    box-shadow: 0rem 0rem 0.5rem 0rem rgb(0, 255, 255);
}

.about__img-overlay1 {
    border-radius: 5px;
    overflow:var(--img-hidden);
    box-shadow: 0rem 0rem 0.5rem 0rem rgb(0, 255, 255);
}

.about__img-one {
    width: 120px;
    border-radius: 5px;
}

.about__img-two {
    width: 180px;
    border-radius: 5px;
}

.about__img-one,
.about__img-two {
    transition: var(--img-transition);
}

.about__img-one:hover,
.about__img-two:hover {
    transform: var(--img-scale);
    transition: 0.4s;
}
@media screen and (max-width: 340px) {
    .about__img-overlay {
        height: auto;
    }

    .about__img-overlay1 {
        height: auto;
    }
}
@media screen and (min-width: 340px) {
    .about__img-overlay {
        height: 160px;
    }

    .about__img-overlay1 {
        height: 250px;
    }
}
@media screen and (min-width: 900px) {
    body {
        margin: 0;
    }

    .about__img-overlay1 {
        height: 250px;
    }
}
@media screen and (min-width: 768px) {
    body {
        margin: 0;
    }
    .section {
        padding: 7rem 0 2rem;
    }
    .about__img-overlay {
        height: 160px;
    }

    .about__img-overlay1 {
        height: 255px;
    }
    .about__container {
        grid-template-columns: repeat(2, 1fr);
        align-items: center;
    }
    .about__data, .about__title {
        text-align: initial;
    }
    .about__title {
        margin-bottom: var(--mb-1-5);
    }
    .about__description {
        margin-bottom: var(--mb-2);
    }
}
@media screen and (min-width: 1024px) {
    .container {
        margin-left: auto;
        margin-right: auto;
    }
    .about__img-overlay {
        height: 300px;
    }

    .about__img-overlay1 {
        height: 405px;
    }
    .about__img-one {
        width: 230px;
    }
    .about__img-two {
        width: 290px;
    }
}
@media screen and (min-width: 1006px) {
    .container {
        max-width: 1024px;
    }
    .about__img-overlay1 {
        height: 400px;
    }
}
@media screen and (min-width: 1200px) {
    .container {
        max-width: 1024px;
    }
}

/* For tall screens on mobiles y desktop*/
@media screen and (min-height: 721px) {
    body {
        margin: 0;
    }
}
</style>
