<template>
        <header>
            <div class="navbar">
                <div id="logo-name">
                    <h1 class="blue-text style-logo">&lt;JOT4</h1><h1 class="teal-text">.dev&gt;</h1>
                </div>
                <div class="hamburguer"></div>
                <ul class="menu">
                    <li><a href="#location_info">Home</a></li>
                    <li><a href="#location_sobreMim">Sobre</a></li>
                    <li><a href="#location_tec">Tecnologias</a></li>
                    <li><a href="#location_projetos">Projetos</a></li>
                </ul> 
            </div>
        </header>
</template>

<script>
    import $ from 'jquery'

    export default {
        name: 'HeaderComponent',
        mounted() {
            $(".hamburguer").click(function() {
                $(this).toggleClass("active");
                $(".menu").toggleClass("active");
            });
        }
    }
</script>

<style lang="sass">
$navy: #053B50
$blue: #176B87
$teal: #64CCC5
$gray: #EEEEEE


.blue-text 
    color: $blue
.teal-text
    color: $teal
.style-logo
    font-style: italic
    font-weight: bold // Analisar porque não esta pegando o bold
#logo-name
    display: flex

header
    width: 100%
    position: absolute
    top: 0
    z-index: 999

    .navbar
        max-width: 80%
        margin: 0 auto

        display: flex
        justify-content: space-between

        .hamburguer
            width: 30px
            height: 30px

            background-color: transparent
            border-radius: 5px
            border: 0

            position: relative
            display: none
            &:after
                content: ""

                position: absolute
                top: 35%
                left: 15%

                width: 70%
                height: 5%
                border-radius: 5px

                background-color: $blue
            
            &:before
                content: ""

                position: absolute
                top: 55%
                left: 15%

                width: 70%
                height: 5%
                border-radius: 5px

                background-color: $blue

        .menu
            list-style: none

            li
                margin-left: 10px 
                float: left

                a
                    position: relative
                    display: block
                    padding: 10px 15px
                    text-decoration: none
                    transition: 0.8s ease
                    color: $navy
                    &:hover
                        color: $teal
                    &:before
                        content: ""
                        position: absolute
                        width: 100%
                        height: 3px
                        bottom: 0
                        left: 0
                        background-color: $teal
                        visibility: hidden
                        -webkit-transform: scaleX(0)
                        transform: scaleX(0)
                        -webkit-transition: all 0.3s ease-in-out 0s
                        transition: all 0.3s ease-in-out 0s
                    &:hover:before 
                        visibility: visible
                        -webkit-transform: scaleX(1)
                        transform: scaleX(1)

@media screen and (max-width: 980px) 
    header
        .navbar
            align-items: center
            .hamburguer
                display: block
                z-index: 999

            .menu
                position: fixed
                top: 0
                right: -100%

                height: 100vh
                margin: 0
                background-color: $navy

                width: 100%
                max-width: 200px

                padding: 100px 20px

                flex-direction: column

                transition: 0.5s ease

                li
                    a
                        color: #dedede
                        margin: 15px 0

            .menu.active
                display: flex
                right: 0         
            .hamburguer.active
                position: none
</style>