<template>
  <div class="container">
    <h1 class="teks">
    Ternyata harus ditambahhin build di nuxt.config.js
  </h1>
  <code>
    build: {
    extend(config) {
      config.resolve.alias['node-fetch-native'] = require.resolve('node-fetch')
    }
  },
  </code>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
<style scoped>
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: black;
  }

  .teks{
    background-color: white;
    padding: 10px;
  }
</style>
