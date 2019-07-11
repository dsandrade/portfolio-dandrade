<template>
  <footer
    class="call-to-action-container section is-primary is-small has-text-centered"
  >
    <div class="container is-narrow">
      <a class="logo" href="#">
        <img
          src="/imgs/d-logo-white.png"
          alt="Daniel Andrade | Backend e Front-end Developer."
          height="48"
        />
      </a>
      <div class="social-icons">
        <p class="field">
          <a
            class="button is-medium"
            href="https://github.com/dsandrade"
            target="#"
          >
            <span class="icon is-small">
              <font-awesome-icon :icon="faGithub" />
            </span>
          </a>
          <a
            class="button is-medium"
            href="https://www.linkedin.com/in/danielsantosandrade/"
            target="#"
          >
            <span class="icon is-small">
              <font-awesome-icon :icon="faLinkedin" />
            </span>
          </a>
          <a
            class="button is-medium"
            href="mailto:dsandrade777@gmail.com"
            target="#"
          >
            <span class="icon is-small">
              <font-awesome-icon :icon="fas.faEnvelope" />
            </span>
          </a>
        </p>
      </div>
      <div class="copyright">
        Create By Daniel Andrade
      </div>
      <div class="made-by-bulma">
        <a href="https://bulma.io">
          <img
            src="https://bulma.io/images/made-with-bulma--white.png"
            alt="Made with Bulma"
            width="163"
            height="31"
          />
        </a>
      </div>
    </div>
  </footer>
</template>

<script>
import { faGithub, faLinkedin } from '@fortawesome/free-brands-svg-icons'
import { fas } from '@fortawesome/free-solid-svg-icons'

export default {
  computed: {
    faGithub() {
      return faGithub
    },
    faLinkedin() {
      return faLinkedin
    },
    fas() {
      return fas
    }
  }
}
</script>

<style>
footer.section.is-small {
  padding: 0 1.5rem 4rem;
}

@media screen and (min-width: 769px) {
  footer.section.is-small {
    padding: 1rem 1.5rem 4rem;
  }
}

.section.is-primary .title {
  color: #fff;
}

@media screen and (min-width: 769px) {
  footer .title {
    max-width: 320px;
  }
}

footer .title {
  font-weight: 300;
  font-size: 1.6rem;
  margin: 2rem auto;
  max-width: 300px;
  opacity: 0.7;
}

footer .social-icons {
  margin: 2.5rem auto 3rem;
}

@media screen and (min-width: 769px) {
  footer .social-icons {
    margin: 2.5rem auto 3.5rem;
  }
}

.section p {
  margin-bottom: 2rem;
}

footer .social-icons a.button.is-medium {
  font-size: 1.05rem;
}

footer .social-icons a.button {
  background-color: transparent;
  color: #fff;
  border-radius: 100%;
  margin: 0 0.2rem;
  height: 47px;
  width: 47px;
  border: 2px solid rgba(255, 255, 255, 0.3);
}

@media screen and (min-width: 769px) {
  footer .social-icons a.button.is-medium {
    font-size: 1.18rem;
  }

  footer .social-icons a.button {
    margin: 0 0.8rem;
  }
}

a,
.button {
  transition: all 0.2s ease-in-out;
  -webkit-transition: all 0.2s ease-in-out;
  font-weight: 400;
}

footer .social-icons a.button .icon.is-small {
  height: 1.4em;
  width: 1.4em;
}

footer .copyright {
  opacity: 0.7;
}

footer .made-by-bulma {
  opacity: 0.6;
  margin-top: 0.7rem;
}
</style>
