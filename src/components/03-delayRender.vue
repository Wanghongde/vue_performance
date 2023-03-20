<template>
  <div>
    <div v-for="item in 20" :key="item" class="box">
      <Heavy v-if="delay(item)"/>
    </div>
  </div>
</template>

<script>
import Heavy from './03-heavyCom.vue'
export default {
  data() {
    return {
      initCount: 0
    }
  },
  components: {
    Heavy
  },
  mounted() {
    const maxCount = 20

    const refreshFrameCount = () => {
      requestAnimationFrame(() => {
        this.initCount += 1

        if(this.initCount < maxCount) {
          refreshFrameCount()
        }
      })
    }

    refreshFrameCount()
  },
  methods: {
    delay(num) {
      return this.initCount >= num
    }
  }
}
</script>

<style scoped>

</style>
