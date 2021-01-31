<template>
  <div class="villa__buttonWhatsapp">
    <img src="/icons/whatsapp.png" @click="handleClick">
  </div>
</template>

<script>
export default {
  methods: {
    handleClick () {
      window.open('https://www.wa.link/izreng', '_blank')
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
