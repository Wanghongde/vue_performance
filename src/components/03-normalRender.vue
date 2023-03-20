<template>
  <div>
    <Heavy v-for="item in 20" :key="item"/>
  </div>
</template>

<script>
import Heavy from './03-heavyCom.vue'
export default {
  components: {
    Heavy
  }
}
</script>

<style scoped>

</style>
