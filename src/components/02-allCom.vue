<template>
  <div >
    <button @click="functionalList = 10000">setFunctionItem</button>
    <button @click="normalList = 10000">setNormalItem</button>

    <div class="box">
      <div class="left">
        <Functional v-for="item in functionalList" :key="item" :num="item"/>
      </div>
      <div class="right">
        <Normal v-for="item in normalList" :key="item" :num="item"/>
      </div>
    </div>

  </div>
</template>

<script>
import Functional from './02-functionCom.vue'
import Normal from './02-normalCom.vue'

export default {
  components: {
    Functional,
    Normal
  },
  data() {
    return {
      functionalList: 0,
      normalList: 0
    }
  }
}
</script>

<style>
.box {
  display: flex;
  margin: 0 auto;
  width: 80vw;
  border: 1px solid #ccc;
  min-height: 200px;
  padding: 20px;
}

.box .left,
.box .right {
  flex: 1;
  border: 1px solid #ccc;
}
</style>
