<template>
  <div>
    <button @click="setInitArr">setInitArr</button>
    <button @click="setFreezeArr">setFreezeArr</button>
    <br>
    {{ initArr.length }}
    {{ freezeArr.length }}
  </div>
</template>

<script>
export default {
  data() {
    return {
      initArr: [],
      freezeArr: []
    }
  },
  methods: {
    initList() {
      let list = []

      for(let i = 0; i < 1000000; i++) {
        list.push({
          id: i,
          uname: '测试名字'
        })
      }

      return list
    },
    setInitArr() {
      this.initArr = this.initList()
    },
    setFreezeArr() {
      this.freezeArr = Object.freeze(this.initList())
    }
  }
}
</script>

<style scoped>

</style>
