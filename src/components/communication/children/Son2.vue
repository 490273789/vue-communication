<template>
    <div class="son1">
        <h2>Im Son2</h2>
        <p>From Parent: {{sonCount}}</p>
        <button @click='changeParent'>ChangeParent</button>
    </div>
</template>

<script>
export default {
  name: 'son2',
  data () {
    return {
      sonCount: 1
    }
  },
  methods: {
    changeParent () {
      this.$parent.pCount += 1
    }
  }
}
</script>

<style scoped>
    .son1 {
        border: 1px solid #c1c1c1;
        padding: 5px;
        margin: 5px;
    }
</style>
