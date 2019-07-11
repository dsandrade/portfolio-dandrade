<template>
  <section
    class="call-to-action-container section call-to-action is-primary has-text-centered"
  >
    <div class="container is-narrow">
      <div class="box">
        <div class="columns level">
          <div class="column level-item">
            <h1 class="title">
              Comece um projeto
            </h1>
          </div>
          <div class="column level-item">
            <p>
              Interessado em trabalhar comigo? Nos deviamos conversar.
            </p>
          </div>
          <div class="column level-item">
            <a
              href="#"
              class="button is-info is-outlined is-rounded is-medium"
              @click.prevent="showModal"
            >
              Vamos Conversar
            </a>
          </div>
        </div>
      </div>
    </div>

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
      this.$refs.contactModal.show()
    }
  }
}
</script>

<style>
.title {
  color: #293347;
  font-weight: 800;
}

.section.clients .client-grid {
  padding-top: 3rem;
}

@media screen and (min-width: 769px) {
  .section.call-to-action .box {
    padding: 3.5rem 1.25rem;
  }
}

.section.call-to-action .box {
  padding: 3.5rem 2rem;
  margin-top: -9rem;
  background-color: #293347;
  box-shadow: 0 5px 5px 0 rgba(0, 0, 0, 0.2), 0 0 0 1px #293347;
}

.section.call-to-action .title,
.section.call-to-action p {
  color: #fff;
  margin-bottom: 0;
}

.section.is-primary .title {
  color: #fff;
}

@media screen and (min-width: 769px) {
  .section.call-to-action .box p {
    font-size: 18px;
  }
}

.section.call-to-action .box .button.is-outlined.is-rounded.is-medium {
  color: #fff;
  padding: 1.25em 2em;
  font-weight: 400;
  border-width: 2px;
}
</style>
