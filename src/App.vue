<template>
  <div class="container">
    <h1>{{ title }}</h1>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      title: 'Vue Components'
    };
  }
}
</script>

<style>
  html {
    box-sizing: border-box;
  }

  body {
    font-family: sans-serif;
    margin: 0;
  }

  .container {
    margin: 0 auto;
    max-width: 1360px;
  }
</style>
