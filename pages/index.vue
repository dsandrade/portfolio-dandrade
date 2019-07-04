<template>
  <div class="index-container">
    <div class="wd-100">
      <Navbar></Navbar>
      <Welcome></Welcome>
      <Presentation></Presentation>
      <Skills></Skills>
      <Clients></Clients>
      <CallToAction></CallToAction>
      <Footer></Footer>
    </div>
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Welcome from '~/components/Welcome.vue'
import Presentation from '~/components/Presentation.vue'
import Skills from '~/components/Skills.vue'
import Clients from '~/components/Clients.vue'
import CallToAction from '~/components/CallToAction.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Navbar,
    Welcome,
    Presentation,
    Skills,
    Clients,
    CallToAction,
    Footer
  }
}
</script>

<style>
.index-container {
  max-width: 100%;
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
