<template>
  <HeaderComponent/>
  <HomeComponent/>
  <SkillsComponent/>
  <ProjectsComponent/>
  <FooterComponent/>
</template>

<script>
import HeaderComponent from './components/header.vue'
import HomeComponent from './components/home.vue'
import SkillsComponent from './components/skills.vue'
import ProjectsComponent from './components/projects.vue'
import FooterComponent from './components/footer.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    HomeComponent,
    SkillsComponent,
    ProjectsComponent,
    FooterComponent,
}
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

body {
  overflow-x: hidden;
  padding: 0;
  margin: 0;
}
</style>
