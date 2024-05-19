<template>
  <div id="app">
    <HeaderPage />
    <BannerComponentProjectDetails />
    <ProjectDetails />
    <FooterPage />
  </div>
</template>

<script>
import HeaderPage from './../../final-examination/src/components/HeaderPage.vue'
import BannerComponentProjectDetails from './components/BannerComponentProjectDetails.vue'
import ProjectDetails from './components/ProjectDetails.vue'
import FooterPage from './../../final-examination/src/components/FooterPage.vue'

export default {
  name: 'App',
  components: {
    HeaderPage,
    BannerComponentProjectDetails,
    ProjectDetails,
    FooterPage
  }
}
</script>
<style>
  a{
    text-decoration: none;
  }

</style>
