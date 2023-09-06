<template>
    <footer class="footer">
        <div class="waves">
            <div class="wave" id="wave1"></div>
            <div class="wave" id="wave2"></div>
            <div class="wave" id="wave3"></div>
            <div class="wave" id="wave4"></div>
        </div>
        <ul class="social-icon">
            <li class="social-icon__item">
                <a href="#" class="social-icon__link">
                    <ion-icon name="logo-email"></ion-icon>
                </a>
            </li>
            <li class="social-icon__item">
                <a href="#" class="social-icon__link">
                    <ion-icon name="logo-whatsapp"></ion-icon>
                </a>
            </li>
            <li class="social-icon__item">
                <a href="#" class="social-icon__link">
                    <ion-icon name="logo-linkedin"></ion-icon>
                </a>
            </li>
            <li class="social-icon__item">
                <a href="#" class="social-icon__link">
                    <ion-icon name="logo-github"></ion-icon>
                </a>
            </li>
        </ul>
        <ul class="menu">
            <li class="menu__item">
                <a href="#" class="menu__link">
                    Home
                </a>
            </li>
            <li class="menu__item">
                <a href="#" class="menu__link">
                    Sobre
                </a>
            </li>
            <li class="menu__item">
                <a href="#" class="menu__link">
                    Tecnologias
                </a>
            </li>
            <li class="menu__item">
                <a href="#" class="menu__link">
                    Projetos
                </a>
            </li>
        </ul>
        <p>&copy;2023 Jota Carvalho | All rights reserved</p>
    </footer>
</template>

<script>
export default {
    name: "FooterComponent"
}
</script>

<style lang="scss"> 
$navy: #053B50;
$blue: #176B87;
$teal: #64CCC5;
$gray: #EEEEEE;


.footer{
    position: relative;
    width: 100%;
    background-color: $gray;
    min-height: 100px;
    padding: 20px 50px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin-top: 200px;
}

.social-icon,
.menu {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 10px 0;
    flex-wrap: wrap;
    gap: 10px;
}

.social-icon__item,
.menu__item {
    list-style: none;
}

.social-icon__link {
    font-size: 2rem;
    color: #fff;
    margin: 0 10px;
    display: inline-block;
    transition: 0.5s;
}

.social-icon__link:hover {
    transform: translateY(-10px);
}

.menu__link {
    font-size: 1.1rem;
    color: $blue;
    margin: 0 10px;
    display: inline-block;
    transition: 0.3s;
    text-decoration: none;
    opacity: 0.75;
    font-weight: 300;
}

.menu__link:hover {
    color: $teal;
    opacity: 1;
}

.footer p {
    color: $blue;
    margin: 15px 0 10px 0;
    font-size: 1rem;
    font-weight: 300;
}

.wave {
    position: absolute;
    top: -100px;
    left: 0;
    width: 100%;
    height: 100px;
    background: url(../assets/wave.png);
    background-size: 1000px 100px;
}

.wave#wave1 {
    z-index: 1000;
    opacity: 1;
    bottom: 0;
    animation: animateWaves 4s linear infinite;
}

.wave#wave2 {
    z-index: 999;
    opacity: 0.5;
    bottom: 10px;
    animation: animate 4s linear infinite !important;
}

.wave#wave3 {
    z-index: 1000;
    opacity: 0.2;
    bottom: 15px;
    animation: animateWaves 3s linear infinite;
}

.wave#wave4 {
    z-index: 999;
    opacity: 0.7;
    bottom: 20px;
    animation: animate 3s linear infinite;
}

@keyframes animateWaves {
    0% {
        background-position-x: 1000px;
    }
    100% {
        background-position-x: 0px;
    }
}

@keyframes animate {
    0% {
        background-position-x: -1000px;
    }
    100% {
        background-position-x: 0px;
    }
}

.social-icon__item .md {
    color: white;
}
</style>