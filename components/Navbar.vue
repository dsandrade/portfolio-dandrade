<template>
  <section class="navbar-component">
    <nav
      class="navbar is-transparent"
      role="navigation"
      aria-label="main navigation"
    >
      <div class="container">
        <div class="navbar-brand">
          <a class="navbar-item" href="#">
            <img
              src="/imgs/d-logo.png"
              alt="Daniel Andrade | Backend e Front-end Developer."
              height="48"
            />
          </a>

          <a
            role="button"
            class="navbar-burger burger"
            aria-label="menu"
            aria-expanded="false"
            data-target="navbarBasicExample"
          >
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div id="navMenu" class="navbar-menu">
          <div class="navbar-end">
            <div class="navbar-item">
              <a
                class="button is-info is-outlined is-rounded"
                @click.prevent="showModal"
              >
                Fale Comigo
              </a>
            </div>
          </div>
        </div>
      </div>
    </nav>

    <ContactModal ref="contactModal"></ContactModal>
  </section>
</template>

<script>
import ContactModal from '~/components/ContactModal.vue'

export default {
  components: {
    ContactModal
  },
  methods: {
    showModal() {
      // eslint-disable-next-line no-console
      console.log('teste')
      this.$refs.contactModal.show()
    }
  }
}
</script>

<style>
.navbar {
  padding: 1.2rem 0;
  box-shadow: none;
  z-index: auto;
}
.navbar .navbar-brand a.navbar-item img {
  max-height: 3rem;
}
.navbar .navbar-menu a.button.is-info.is-outlined {
  border-width: 2px;
  font-weight: 400;
  font-size: 18px;
  padding: 1.2rem;
}
.navbar.container {
  align-items: stretch;
  display: flex;
  min-height: 3.25rem;
  width: 100%;
}
</style>
