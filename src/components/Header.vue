<template>
  <div class="hello">
      <h1>Header</h1>
      <p>{{headerMsg}}</p>
  </div>
</template>

<script>
export default {
    name: 'Header',
    props: {
        headerMsg: String
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    div {
        background-color: lightgreen;
    }
</style>
