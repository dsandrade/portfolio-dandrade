<template>
  <section class="skills-component section skills has-text-centered">
    <div class="container is-narrow">
      <div class="box">
        <div class="content">
          <div class="columns is-centered">
            <div class="column">
              <figure class="image">
                <img
                  class="is-skill-icon"
                  src="/imgs/designer.svg"
                  alt="designer image"
                />
              </figure>
              <h1 class="title is-size-4 is-spaced">
                Back-end Developer
              </h1>
              <p>
                Eu gosto de escrever códigos bem estruturados, com os design
                patterns corretos, para que o código seja sempre reutilizável e
                fácil de dar manutenção ou desenvolver novas funcionalidades.
              </p>
              <p class="list-title has-text-primary has-text-weight-normal">
                Linguagens que utilizo:
              </p>
              <p>PHP, Laravel, Slim, Lumen, Node Js</p>
            </div>
            <div class="column">
              <figure class="image">
                <img
                  class="is-skill-icon"
                  src="/imgs/frontend.svg"
                  alt="frontend image"
                />
              </figure>
              <h1 class="title is-size-4 is-spaced">
                Front-end Developer
              </h1>
              <p>
                Acredito sempre em códigos bem estruturados, reutilizáveis e
                componentizados. Gosto sempre de transformar ideias em realidade
                no navegador
              </p>
              <p class="list-title has-text-primary has-text-weight-normal">
                Languages I speak:
              </p>
              <p>HTML, CSS, Sass, Less, Stylus, Javascript, VueJS</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.title {
  font-weight: 800;
}

.section.skills {
  margin-top: -14rem;
  padding-bottom: 1rem;
}

.section.skills .box {
  padding: 0;
}

.section.skills .box .content .columns {
  margin-left: 0;
  margin-right: 0;
}

.section.skills .box .content .columns .column {
  padding: 50px 30px;
  border-bottom: 1px solid #e6ecf8;
  border-right: 0 solid #e6ecf8;
}

@media screen and (min-width: 769px) {
  .section.skills .box .content .columns .column {
    border-bottom: 0 solid #e6ecf8;
    border-right: 1px solid #e6ecf8;
    padding: 60px 35px;
  }
}

.section.skills .box .content .columns .column figure.image {
  margin: 0 auto 2em;
}

.section.skills .box .content .columns .column figure.image img.is-skill-icon {
  height: 48px;
  width: auto;
}

@media screen and (min-width: 769px) {
  .section.skills .box .content .columns .column p {
    font-size: 18px;
  }
}

.content p:not(:last-child) {
  margin-bottom: 2em;
}

.section p {
  margin-bottom: 2rem;
}

.content p {
  font-size: 18px;
}

.section.skills .box .content .columns .column p.list-title {
  margin-top: 50px;
  margin-bottom: 8px;
}

.section.skills .box .content .columns .column p {
  font-weight: 300;
}

@media screen and (min-width: 769px) {
  .section.skills .box .content .columns .column p {
    font-size: 18px;
  }
}

.section.skills .box .content .columns .column ul {
  list-style: none;
  margin-left: 0;
  margin-top: 0;
}

.section.skills .box .content .columns .column ul li {
  font-weight: 300;
}

@media screen and (min-width: 769px) {
  .section.skills .box .content .columns .column ul li {
    font-size: 18px;
  }
}
</style>
