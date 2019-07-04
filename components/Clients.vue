<template>
  <section
    class="clients-component section clients is-medium is-white has-text-centered"
  >
    <div class="container is-narrow">
      <div class="columns is-centered">
        <div class="column is-half">
          <h1 class="title is-size-3-desktop is-size-4-tablet is-size-5-mobile">
            Tenho orgulho de já ter colaborado com algumas empresas incríveis:
          </h1>
        </div>
      </div>
      <div class="client-grid is-mobile">
        <div class="columns is-multiline is-mobile">
          <div class="column is-half-mobile is-one-third-tablet">
            <figure class="image is-2x1">
              <img
                class="client-logo"
                alt="Empresa Tray Tecnologia"
                src="/imgs/tray.png"
              />
            </figure>
          </div>
          <div class="column is-half-mobile is-one-third-tablet">
            <figure class="image is-2x1">
              <img
                class="client-logo"
                alt="Empresa Boa Vista SCPC"
                src="/imgs/boavista.gif"
              />
            </figure>
          </div>
          <div class="column is-half-mobile is-one-third-tablet">
            <figure class="image is-2x1">
              <img
                class="client-logo pedfarma-logo"
                alt="Empresa PedFarma"
                style="width: 25% !important;"
                src="/imgs/pedfarma.svg"
              />
            </figure>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.title {
  color: #293347;
  font-weight: 800;
}

.section.clients .client-grid {
  padding-top: 3rem;
}

.image.is-2x1 img {
  width: 50% !important;
}

.image.is-2x1 {
  display: flex;
  justify-content: center;
  align-items: center;
}

.pedfarma-logo {
  margin-bottom: 40%;
}

@media screen and (min-width: 769px) {
  .pedfarma-logo {
    margin-bottom: 25%;
  }
}
</style>
