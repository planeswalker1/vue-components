<template>
  <div class="container">
    <appHeader></appHeader>
    <bros></bros>
    <appFooter></appFooter>
  </div>
</template>

<script>
import Bros from './components/Bros.vue'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    bros: Bros,
    appHeader: Header,
    appFooter: Footer
  },
  data: function () {
    return {
      title: 'Click on a name to show their specialty'
    };
  }
}
</script>

<style>
  html {
    box-sizing: border-box;
  }

  *,
  *:before,
  *:after {
    box-sizing: inherit;
  }

  html,
  body {
     height: 100%;
  }

  body {
    font-family: sans-serif;
    margin: 0;
  }

  .container {
    display: flex;
    flex-direction: column;
    margin: 0 auto;
    min-height: 100%;
    max-width: 1360px;
  }

  h1,
  h2,
  p {
    color: #222;
    text-align: center;
  }
</style>
