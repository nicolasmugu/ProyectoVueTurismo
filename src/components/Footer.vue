<template>
    <!--==================== FOOTER ====================-->
        <footer class="footer section">
            <div class="footer__container container grid">
                <div class="footer__content grid">
                    <div class="footer__data">
                        <h3 class="footer__title">Viaje</h3>
                        <p class="footer__description">Viaja con nosotros tu elgies el<br> destino,
                            nosotros te ofrecemos la mejor experiencia <br> experience.
                        </p>
                        <div>
                            <a href="https://www.facebook.com/" target="_blank" class="footer__social">
                                <i class="ri-facebook-box-fill"></i>
                            </a>
                            <a href="https://twitter.com/" target="_blank" class="footer__social">
                                <i class="ri-twitter-fill"></i>
                            </a>
                            <a href="https://www.instagram.com/" target="_blank" class="footer__social">
                                <i class="ri-instagram-fill"></i>
                            </a>
                            <a href="https://www.youtube.com/" target="_blank" class="footer__social">
                                <i class="ri-youtube-fill"></i>
                            </a>
                        </div>
                    </div>

                    <div class="footer__data">
                        <h3 class="footer__subtitle">Información</h3>
                        <ul>
                            <li class="footer__item">
                                <a href="" class="footer__link">Sobre nosotros</a>
                            </li>
                            <li class="footer__item">
                                <a href="" class="footer__link">Características</a>
                            </li>
                            <li class="footer__item">
                                <a href="" class="footer__link">Novedades & Blog</a>
                            </li>
                        </ul>
                    </div>

                    <div class="footer__data">
                        <h3 class="footer__subtitle">Empresa</h3>
                        <ul>
                            <li class="footer__item">
                                <a href="" class="footer__link">Equipo</a>
                            </li>
                            <li class="footer__item">
                                <a href="" class="footer__link">Planes y Precios</a>
                            </li>
                            <li class="footer__item">
                                <a href="" class="footer__link">Conviertete en miembro</a>
                            </li>
                        </ul>
                    </div>

                    <div class="footer__data">
                        <h3 class="footer__subtitle">Soporte</h3>
                        <ul>
                            <li class="footer__item">
                                <a href="" class="footer__link">FAQs</a>
                            </li>
                            <li class="footer__item">
                                <a href="" class="footer__link">Centro de apoyo</a>
                            </li>
                            <li class="footer__item">
                                <a href="" class="footer__link">Contactenos</a>
                            </li>
                        </ul>
                    </div>
                </div>

                <div class="footer__rights">
                    <p class="footer__copy">&#169; Todos los derechos reservados.</p>
                    <div class="footer__terms">
                        <a href="#" class="footer__terms-link">Terminos & Condiciones</a>
                        <a href="#" class="footer__terms-link">Política de Privacidad</a>
                    </div>
                </div>
            </div>
        </footer>
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


/*=============== FOOTER ===============*/
.ri-youtube-fill:hover{
    color: rgba(196, 48, 43,1)
}
.footer__container {
    row-gap: 5rem;
}

.footer__content {
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    row-gap: 2rem;
}

.footer__title,
.footer__subtitle {
    font-size: var(--h3-font-size);
}

.footer__title {
    margin-bottom: var(--mb-0-5);
}

.footer__description {
    margin-bottom: var(--mb-2);
}

.footer__social {
    font-size: 1.25rem;
    color: var(--title-color);
    margin-right: var(--mb-1-25);
}

.footer__subtitle {
    margin-bottom: var(--mb-1);
}

.footer__item {
    margin-bottom: var(--mb-0-75);
}

.footer__link {
    color: var(--text-color);
}

.footer__link:hover {
    color: rgb(0, 255, 255);
}

.footer__rights {
    display: flex;
    flex-direction: column;
    row-gap: 1.5rem;
    text-align: center;
}

.footer__copy, .footer__terms-link {
    font-size: var(--small-font-size);
    color: var(--text-color-light);
}

.footer__terms {
    display: flex;
    column-gap: 1.5rem;
    justify-content: center;
}

.footer__terms-link:hover {
    color: var(--text-color);
}


::-webkit-scrollbar-thumb:hover {
    background-color: var(--text-color-light);
}

/*=============== MEDIA QUERIES ===============*/
/* For small devices */
@media screen and (max-width: 340px) {
    .place__container {
        grid-template-columns: max-content;
        justify-content: center;
    }
    .experience__content {
        padding: 0;
    }
    .experience__overlay:nth-child(1) {
        width: 190px;
    }
    .experience__overlay:nth-child(2) {
        width: 80px;
    }

    .experience__img,
    .video__container {
        padding: 0;
    }
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
