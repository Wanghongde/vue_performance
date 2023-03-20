<template functional>
  <div>
    <h2>functional com  ----  {{ props.num }}</h2>
  </div>
</template>

<script>
export default {
  functional: true,
  props: {
    num: Number
  }
}
</script>

<style scoped>

</style>
