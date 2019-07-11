<template>
  <section class="contact-modal">
    <div class="modal" :class="{ 'is-active': isActive }">
      <div class="modal-background" @click.prevent="close"></div>
      <div class="modal-card">
        <section class="modal-card-body">
          <div class="is-form">
            <div class="is-white has-text-centered">
              <div class="container">
                <div class="columns is-centered">
                  <div class="column is-three-quarters">
                    <h1
                      class="title is-spaced is-size-1-desktop is-size-2-tablet is-size-3-mobile title-black"
                    >
                      Obrigado pela atenção, entre em contato comigo pelo meu
                      email:
                    </h1>
                    <h2
                      class="subtitle is-spaced is-size-1-desktop is-size-2-tablet is-size-3-mobile title-black"
                    >
                      dsandrade777@gmail.com
                    </h2>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      isActive: false
    }
  },
  methods: {
    show() {
      this.isActive = true
    },
    close() {
      this.isActive = false
    }
  }
}
</script>

<style>
.title-black {
  color: #293347 !important;
}

.modal-content,
.modal-card {
  width: 20rem;
}

@media screen and (max-width: 768px) {
  .is-size-3-mobile {
    font-size: 1.5rem !important;
  }
}

@media screen and (min-width: 769px), print {
  .modal-content,
  .modal-card {
    width: 60rem;
  }
}

.is-active {
  display: block;
}

.is-form .container {
  padding: 0 20px;
}

.is-form-page .container form {
  max-width: 640px;
  margin: 32px auto 0;
}

@media screen and (min-width: 769px) {
  .is-form-page .container form {
    margin: 60px auto 0;
  }
}

.is-form-page .container form button {
  margin: 20px 0 80px;
  border-width: 2px;
  font-weight: 400;
  height: auto;
}

.button.is-dsandrade {
  background-color: #209cee;
  border-color: transparent;
  color: #fff;
}
</style>
