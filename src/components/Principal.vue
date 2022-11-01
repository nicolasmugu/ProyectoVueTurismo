<template>
        <!--==================== HOME ====================-->
    <section class="home" id="home">
        <img src="https://www.wallpapertip.com/wmimgs/51-513276_san-andres-colombia-hd.jpg"  alt="" class="home__img">
        <div class="home__container container grid">
            <div class="home__data">
                <a href="#discover"><span class="home__data-subtitle">Descubre tu lugar</span></a>
                    <h1 class="home__data-title">Viaja por los más <br>  <b> &nbsp;&nbsp;hermosos sitios  <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;turísticos </b></h1>
                <a href="#discover" class="button">Explorar</a>
            </div>
            <div class="home__social">
                <a href="https://www.facebook.com/" target="_blank" class="home__social-link">
                    <i class="ri-facebook-box-fill"></i>
                </a>
                <a href="https://www.instagram.com/" target="_blank" class="home__social-link">
                    <i class="ri-instagram-fill"></i>
                </a>
                <a href="https://twitter.com/" target="_blank" class="home__social-link">
                    <i class="ri-twitter-fill"></i>
                </a>
            </div>
            <div class="home__info">
                <div>
                    <span class="home__info-title">5 mejores lugares para visitar</span>
                    <a href="#place" class="button1 button--flex1 button--link home__info-button">
                            M&aacute;s <i class="ri-arrow-right-line"></i>
                    </a>
                </div>
                <div class="home__info-overlay">
                    <img src="./../assets/img/home2.jpg" alt="" class="home__info-img">
                </div>
            </div>
        </div>
    </section>
</template>

<script>

</script>
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

.container {
    max-width: 968px;
    margin-left: var(--mb-1);
    margin-right: var(--mb-1);
}
.grid {
    display: grid;
    gap: 1.5rem;
}
/*=============== HOME ===============*/
.home__img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    object-fit: cover;
    object-position: 83%;
    filter: brightness(75%);
}

.home__container {
    position: relative;
    height: calc(100vh - var(--header-height));
    align-content: center;
    row-gap: 3rem;
}

.home__data-subtitle,
.home__data-title,
.home__social-link,
.home__info {
    color: var(--white-color);
}

.home__data-subtitle {
    display: block;
    font-weight: var(--font-semi-bold);
    margin-bottom: var(--mb-0-75);
}

.home__data-title {
    font-size: var(--biggest-font-size);
    font-weight: var(--font-medium);
    margin-bottom: var(--mb-2-5);
}

.home__social {
    display: flex;
    flex-direction: column;
    row-gap: 1.5rem;
}

.home__social-link {
    font-size: 1.2rem;
    width: max-content;
}

.home__info {
    background-color: var(--first-color);
    display: flex;
    padding: 1.5rem 1rem;
    align-items: center;
    column-gap: .5rem;
    position: absolute;
    right: 0;
    bottom: 1rem;
    width: 228px;
    border-radius: 5px;
}

.home__info-title {
    display: block;
    font-size: var(--small-font-size);
    font-weight: var(--font-semi-bold);
    margin-bottom: var(--mb-0-75);
}

.home__info-button {
    font-size: var(--smaller-font-size);
}
.home__info-button:hover {
    color: rgb(0, 255, 255);
}
.ri-facebook-box-fill:hover{
    color:rgb(59,89,152);
}
.ri-instagram-fill:hover {
    color:rgb(255, 102, 255);
}
.ri-twitter-fill:hover{
    color: rgb(0, 255, 255);
}
.home__info-overlay {
    overflow: var(--img-hidden);
}
.home__info-img {
    width: 145px;
    transition: var(--img-transition);
}
.home__info-img:hover {
    transform: var(--img-scale);
}
/*=============== BUTTONS ===============*/
.button {
    display: inline-block;
    background-color: var(--first-color);
    color: var(--white-color);
    padding: 1rem 2rem;
    font-weight: var(--font-semi-bold);
    transition: .3s;
    border-radius: 50px;
}

.button:hover {
    background-color: var(--first-color-alt);
    color: rgb(0, 255, 255);
    box-shadow: 0rem 0rem 0.5rem -0.1rem rgb(0, 255, 255);
}
.button1 {
    font-weight: var(--font-semi-bold);
    display: inline-block;
    color:var(--white-color);
    transition: .3s;
}
.button1:active {
    transform: scale(0.6);
    transition: 0.2s;
    box-shadow: 0rem 0rem 20rem 0rem rgb(255, 255, 255);
}
.button:active{
    transform: scale(0.7);
    transition: 0.4s;
    box-shadow: 0rem 0rem 20rem 0rem rgb(255, 255, 255);
}

.button--flex {
    display: flex;
    align-items: center;
    column-gap: .25rem;
}
.button--flex {
    display: flex;
    align-items: center;
    column-gap: .25rem;
}

.button--link {
    background: none;
    padding: 0;
}

.button--link:hover {
    background: none;
}
@media screen and (max-width: 340px) {
    .home__info {
        width: 190px;
        padding: 1rem;
    }
}
@media screen and (min-width: 1024px) {
    .container {
            margin-left: auto;
            margin-right: auto;
        }
    .home__container {
        grid-template-rows: 2fr .5fr;
    }
    .home__info {
        width: 328px;
        grid-template-columns: 1fr 2fr;
        column-gap: 2rem;
    }
    .home__info-title {
        font-size: var(--normal-font-size);
    }
    .home__info-img {
        width: 240px;
    }
}
@media screen and (min-width: 768px) {
    body {
        margin: 0;
    }
    .home__container {
        height: 100vh;
        grid-template-rows: 1.8fr .5fr;
    }
    .home__data {
        align-self: flex-end;
    }
    .home__social {
        flex-direction: row;
        align-self: flex-end;
        margin-bottom: 3rem;
        column-gap: 2.5rem;
    }
    .home__info {
        bottom: 3rem;
    }
    .home__container {
        height: 100vh;
        grid-template-rows: 1.8fr .5fr;
    }
    .home__data {
        align-self: flex-end;
    }
    .home__social {
        flex-direction: row;
        align-self: flex-end;
        margin-bottom: 3rem;
        column-gap: 2.5rem;
    }
    .home__info {
        bottom: 3rem;
    }
}
@media screen and (min-width:940px ) {
    .home__data {
        margin-top: 110px;
    }
}
@media screen and (min-width: 1200px) {
    .container {
        max-width: 1024px;
    }
    .home__data {
        margin-top: 110px;
    }
}
@media screen and (min-height: 721px) {
    body {
        margin: 0;
    }
    .home__container, .home__img {
            height: 640px;
        }
}

</style>
