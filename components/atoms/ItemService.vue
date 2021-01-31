<template>
  <div>
    <a-card v-if="item !== null">
      <img
        slot="cover"
        alt="example"
        :src="item.img"
      >
      <a-card-meta :title="item.title">
        <template slot="description">
          {{ item.description }}
        </template>
      </a-card-meta>
    </a-card>
  </div>
</template>

<script>
export default {
  props: {
    item: {
      type: Object,
      default: null
    }
  }
}
</script>
