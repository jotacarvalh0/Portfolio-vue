<template>
    <h1 class="title-box">SKILLS</h1>
    <section class="skills-box">
        <div class="skill">
            <img src="../../public/skills/angular.svg" alt="Icone Angular">
            <ul class="skill-description">
                <h4 class="skill-name">Angular</h4>
                <p class="skill-status">Intermediário</p>
            </ul>
        </div>
        <div class="skill">
            <img src="../../public/skills/vue.svg" alt="Icone Vue">
            <ul class="skill-description">
                <h4 class="skill-name">Vue</h4>
                <p class="skill-status">Intermediário</p>
            </ul>
        </div>
        <div class="skill">
            <img src="../../public/skills/react.svg" alt="Icone React">
            <ul class="skill-description">
                <h4 class="skill-name">React</h4>
                <p class="skill-status">Básico</p>
            </ul>
        </div>

        <div class="skill">
            <img src="../../public/skills/javascript.svg" alt="Icone Javascript">
            <ul class="skill-description">
                <h4 class="skill-name">JavaScript</h4>
                <p class="skill-status">Avançado</p>
            </ul>
        </div>
        <div class="skill">
            <img src="../../public/skills/typescript.svg" alt="Icone Typescript">
            <ul class="skill-description">
                <h4 class="skill-name">TypeScript</h4>
                <p class="skill-status">Intermediário</p>
            </ul>
        </div>
        <div class="skill">
            <img src="../../public/skills/git.svg" alt="Icone Git">
            <ul class="skill-description">
                <h4 class="skill-name">Git</h4>
                <p class="skill-status">Avançado</p>
            </ul>
        </div>

        <div class="skill">
            <img src="../../public/skills/sass.svg" alt="Icone Sass">
            <ul class="skill-description">
                <h4 class="skill-name">Sass</h4>
                <p class="skill-status">Avançado</p>
            </ul>
        </div>
        <div class="skill">
            <img src="../../public/skills/go.svg" alt="Icone Go">
            <ul class="skill-description">
                <h4 class="skill-name">Go</h4>
                <p class="skill-status">Básico</p>
            </ul>
        </div>
        <div class="skill">
            <img src="../../public/skills/nodejs.svg" alt="Icone NodeJs">
            <ul class="skill-description">
                <h4 class="skill-name">NodeJS</h4>
                <p class="skill-status">Básico</p>
            </ul>
        </div>
    </section>
</template>

<script>
    export default {
        name:'SkillsComponent'
    }
</script>

<style lang="sass">
$navy: #053B50
$blue: #176B87
$teal: #64CCC5
$gray: #EEEEEE

*
    font-family: Arial, Helvetica, sans-serif

.title-box
    font-weight: bold
    font-size: 40px
    text-shadow: 0px -8px 5px rgba(5,59,80,0.34)

.skill
    img
        width: 30px
        height: 30px

</style>