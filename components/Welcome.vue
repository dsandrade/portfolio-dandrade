<template>
  <section class="welcome-component hero is-white has-text-centered">
    <div class="hero-body">
      <div class="container">
        <div class="columns is-centered">
          <div class="column">
            <h1
              class="title is-spaced is-size-1-desktop is-size-2-tablet is-size-3-mobile"
            >
              Desenvolvedor Back-end e Front-end
            </h1>
            <h2 class="subtitle is-size-4-desktop">
              Eu desenvolvo códigos simples e otimizados, isso é o que amo fazer
            </h2>
            <img class="avatar" src="/imgs/avatar-coffee.png" />
          </div>
        </div>
      </div>
    </div>
    <div class="hero-foot">
      <div class="container">
        <img class="is-bottom" src="/imgs/hero.png" alt="Computer Images" />
      </div>
    </div>
  </section>
</template>

<style>
.title {
  color: #293347;
  display: block;
  font-weight: 800;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  line-height: 1.5;
}

.hero-foot {
  padding: 0 1.5rem;
}

.hero-foot img.is-bottom {
  margin-bottom: -0.4rem;
}

@media screen and (min-width: 769px) {
  .hero-foot img.is-bottom {
    margin-bottom: -0.45rem;
    max-width: 860px;
  }
}
</style>
