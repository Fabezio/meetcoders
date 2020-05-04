<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">
        Rencontrez les codeurs
      </h1>
      <h2 class="subtitle">
        Une App pour gérer les codeurs,
        <br />une App pour rencontrer des codeurs
      </h2>
      <div class="links">
        <a href="https://nuxtjs.org/" target="_blank" class="button--green">
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey"
        >
          GitHub
        </a>
      </div>

      <h1 class="coder-list">
        Tous les codeurs
      </h1>

      <div class="coder-container">
        <div class="blank"></div>
        <div class="coder-info">
          <h3>Coder Name</h3>
          <p>Future coder description can go here.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
export default {
  layout: 'main',
  components: {
    Logo
  }
}
</script>

<style>
.blank {
  width: 100px;
  height: 100px;
  border: 1px solid lightgray;
  border-radius: 5px;
}
.coder-list {
  margin-top: 1em;
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
h1 {
  margin-bottom: 1em;
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 48px;
  color: #35495e;
  letter-spacing: 1px;
}
.links {
  padding-top: 15px;
}
.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
</style>
