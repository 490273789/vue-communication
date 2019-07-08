<template>
  <div class="wrapper">
    <h2>Chilid2</h2>
    <p>{{demo}}</p>
  </div>
</template>

<script>
export default {
  inject: ['for'],
  data () {
    return {
      demo: this.for
    }
  }
}
</script>

<style scoped>
.wrapper {
  border: 1px solid #c1c1c1;
  margin: 5px;
  padding: 5px;
}
</style>
