<template>
  <div class="box">
    <div class="son" v-for="item in 8000" :key="item"></div>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
.box {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  width: 800px;
  height: 800px;
  border: 1px solid red;
}

.box .son {
  width: 2px;
  height: 2px;
  margin: 1px;
  background: #ccc;
}
</style>
