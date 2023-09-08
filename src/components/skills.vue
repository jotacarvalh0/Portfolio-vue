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

.skills-box
    width: 80%
    margin: 0 auto
    gap: 3rem 1rem
    z-index: 1000
    margin-top: 5rem

    display: grid
    place-items: center
    grid-template-columns: 1fr 1fr 1fr

.skill
    display: flex
    flex-direction: row
    align-items: center

    font-size: 1.25rem
    gap: 0.1rem
    color: $navy
    transition: all 0.3s ease 0s
    text-transform: uppercase
    font-weight: 400
    img
        height: 4.375rem
        filter: grayscale(100%)
        transition: all 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275)

.skill-name
    letter-spacing: 0.1rem
    line-height: 1rem
    font-weight: 600
    padding: 0px 0.25rem 0px 0.25rem

.skill-status
    max-width: 120px
    font-size: 16px
    text-transform: capitalize
    text-align: center
    border: 1px solid none
    color: $gray
    background-color: $navy
    padding: 0.75rem
    margin-left: 12px
    border-radius: 12px
    font-weight: 600
    visibility: hidden
    &:hover
        transform: scale(1.1)
        transition: all 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275)
        filter: drop-shadow(#666 10px 10px 5px)

.skills-box div:hover img
    filter: none
    height: 7rem
    transition: all 1s cubic-bezier(0.175, 0.885, 0.32, 1.275)


.skills-box div:hover p
    visibility: visible
</style>