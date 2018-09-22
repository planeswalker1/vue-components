<template>
  <footer>
    <p>{{ copyright }}</p>
  </footer>
</template>

<script>
export default {
  data: function () {
    return {
      copyright: 'Copyright 2018 Vue Components'
    };
  }
}
</script>

<style scoped>
  footer {
    background-color: #222;
    padding: 6px;
  }

  p {
    color: #add8e6;
  }
</style>
