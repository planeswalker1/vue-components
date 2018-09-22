<template>
  <main>
    <h2>{{ title }}</h2>
    <ul class="bros">
      <li v-on:click="bro.show = !bro.show" v-for="bro in bros">
        <h2>{{ bro.name }}</h2>
        <p v-show="bro.show">{{ bro.specialty }}</p>
      </li>
    </ul>
    <h2>Some Cool Links</h2>
    <ul class="links">
      <li><a href="https://colorlessenergy.github.io/">Ultra Cool Website</a></li>
      <li><a href="https://planeswalker1.github.io/">My Website</a></li>
    </ul>
  </main>
</template>

<script>
export default {
  data: function () {
    return {
      title: 'Click on a name to show their specialty',
      bros: [
        {name: 'Christian', specialty: 'Magic the Gathering', show: false},
        {name: 'Daniel', specialty: 'Vue Components', show: false},
        {name: 'Brian', specialty: 'javaScript Wizard', show: false},
        {name: 'Angel', specialty: 'Pixel Worlds', show: false},
        {name: 'David', specialty: 'Fornite', show: false},
      ]
    };
  }
}
</script>

<style scoped>
  main {
    flex: 1;
    margin: 40px 0;
    padding: 0 20px;
  }

  .bros,
  .links {
    list-style-type: none;
    padding: 0;
    justify-content: center;
  }

  .bros {
    /* display: flex; */
    /* flex-wrap: wrap; */
    display: grid;
    grid-template-columns: 300px 300px;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 20px;
  }

  .bros li {
    border: 1px solid #222;
    padding: 30px;
    cursor: pointer;
  }

  .links {
    display: flex;
    width: 100%;
  }

  .links li {
    margin-right: 10px;
  }

  a {
    color: #007bff;
    text-decoration: none;
    padding: 10px 15px;
  }

  a:hover {
    color: #0056b3;
    text-decoration: underline;
  }

  @media only screen and (max-width: 960px) {
    ul {
      grid-template-columns: 1fr;
      grid-template-rows: repeat(5, 1fr);
    }
  }
</style>
