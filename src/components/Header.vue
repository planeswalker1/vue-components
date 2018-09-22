<template>
  <header>
    <h1>{{ title }}</h1>
  </header>
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

<style scoped>
  header {
    background-color: #add8e6;
    padding: 10px;
  }
</style>
