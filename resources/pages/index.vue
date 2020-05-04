<template lang="pug">
  .container
    div
      Logo
      h1.title
        | Rencontrez les codeurs
      h2.subtitle
        | Une App pour gérer les codeurs,
        br
        | une App pour rencontrer des codeurs
      .links
        a.button--green(href='#', target='_self') Find Coders
        a.button--grey(href='#', target='_self') Find Coders by languages

      h1.coder-list
        | Tous les codeurs
      .coder-container
        .blank
        .coder-info
          h3 Coder Name
          p Future coder description can go here.

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
