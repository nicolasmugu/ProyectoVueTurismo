<template>
    <!--==================== EXPERIENCE ====================-->
            <section class="experience section">
                <h2 class="section__title">Con Nuestra Experiencia <br> Nosotros Te Serviremos</h2>

                <div class="experience__container container grid">
                    <div class="experience__content grid">
                        <div class="experience__data">
                            <h2 class="experience__number">20</h2>
                            <span class="experience__description">Años <br> Experiencia</span>
                        </div>

                        <div class="experience__data">
                            <h2 class="experience__number">75</h2>
                            <span class="experience__description">Tours <br> completados</span>
                        </div>
                        <div class="experience__data">
                            <h2 class="experience__number">650+</h2>
                            <span class="experience__description"> Destinos <br> Turísticos</span>
                        </div>
                    </div>
                    <div class="experience__img grid">
                        <div class="experience__overlay">
                            <img src="./../assets/img/experience1.jpg" alt="" class="experience__img-one">
                        </div>
                        <div class="experience__overlay">
                            <img src="./../assets/img/experience2.jpg" alt="" class="experience__img-two">
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





/*=============== EXPERIENCE ===============*/
.experience__container {
    row-gap: 2.5rem;
    justify-content: center;
    justify-items: center;
}

.experience__content {
    grid-template-columns: repeat(3, 1fr);
    column-gap: 1rem;
    justify-items: center;
    padding: 0 2rem;
}

.experience__number {
    font-size: var(--h2-font-size);
    font-weight: var(--font-semi-bold);
    margin-bottom: var(--mb-0-5);
}

.experience__description {
    font-size: var(--small-font-size);
}

.experience__img {
    position: relative;
    padding-bottom: 2rem;
}

.experience__img-one, 
.experience__img-two {
    transition: var(--img-transition);
}

.experience__img-one:hover, 
.experience__img-two:hover {
    transform: var(--img-scale);
}

.experience__overlay {
    overflow: var(--img-hidden);
}

.experience__overlay:nth-child(1) {
    width: 263px;
    margin-right: 2rem;
}

.experience__overlay:nth-child(2) {
    width: 120px;
    position: absolute;
    top: 2rem;
    right: 0;
}


    /* For medium devices */
@media screen and (min-width: 568px) {
    .video__container {
        display: grid;
        grid-template-columns: .6fr;
        justify-content: center;
    }
    .place__container {
        grid-template-columns: repeat(3, max-content);
    }
    .subscribe__form {
        width: 470px;
        margin: 0 auto;
    }
}

@media screen and (min-width: 768px) {
    body {
        margin: 0;
    }
    
    .section {
        padding: 7rem 0 2rem;
    }
    .discover__container {
        width: 610px;
        margin-left: auto;
        margin-right: auto;
    }
    .discover__container,
    .place__container {
        padding-top: 2rem;
    }
    .experience__overlay:nth-child(1) {
        width: 363px;
        margin-right: 4rem;
    }
    .experience__overlay:nth-child(2) {
        width: 160px;
    }
    .subscribe__bg {
        background: none;
        padding: 0;
    }
    .subscribe__container {
        background-color: var(--first-color-second);
        padding: 3.5rem 0;
    }
    .subscribe__input {
        padding: 0 .5rem;
    }
    .footer__rights {
        flex-direction: row;
        justify-content: space-between;
    }
    }

/* For large devices */
@media screen and (min-width: 1024px) {
    .container {
        margin-left: auto;
        margin-right: auto;
    }
    .discover__card {
        width: 237px;
    }
    .discover__container {
        width: 700px;
    }
    .discover__data {
        left: 1.5rem;
        bottom: 2rem;
    }
    .discover__title {
        font-size: var(--h2-font-size);
    }
    .experience__content {
        margin: var(--mb-1) 0;
        column-gap: 3.5rem;
    }
    .experience__overlay:nth-child(1) {
        width: 463px;
        margin-right: 7rem;
    }
    .experience__overlay:nth-child(2) {
        width: 220px;
        top: 3rem;
    }
    .video__container {
        grid-template-columns: .7fr;
    }
    .video__description {
        padding: 0 8rem;
    }
    .place__container {
        gap: 3rem 2rem;
    }
    .place__card, .place__img {
        height: 263px;
        
    }
    .footer__content {
        justify-items: center;
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
