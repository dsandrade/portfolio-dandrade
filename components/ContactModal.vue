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
                      Obrigado por entrar em contato comigo. Como posso
                      ajudá-lo?
                    </h1>
                  </div>
                </div>
              </div>
            </div>
            <div class="is-white">
              <div class="container">
                <form id="form" action="#" method="POST" accept-charset="UTF-8">
                  <div class="columns is-centered">
                    <div class="column is-half">
                      <div class="field">
                        <label class="label" for="name">
                          Nome
                        </label>
                        <div class="control is-expanded">
                          <input
                            type="text"
                            class="input is-large"
                            name="name"
                            id="name"
                            required
                          />
                        </div>
                      </div>
                    </div>
                    <div class="column is-half">
                      <div class="field">
                        <label class="label" for="email">
                          Email
                        </label>
                        <div class="control is-expanded">
                          <input
                            type="email"
                            class="input is-large"
                            id="email"
                            name="email"
                            required
                          />
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="columns is-centered">
                    <div class="column">
                      <div class="field">
                        <label class="label" for="message">Mensagem</label>
                        <div class="control is-expanded">
                          <textarea
                            class="textarea is-large"
                            name="message"
                            id="message"
                            rows="5"
                            required
                          ></textarea>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="columns is-centered">
                    <div class="column">
                      <button class="button is-dsandrade">
                        Enviar
                      </button>
                    </div>
                  </div>
                </form>
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
