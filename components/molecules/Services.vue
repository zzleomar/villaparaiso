<template>
  <div class="villa__services">
    <h4 class="villa__services--h4">
      Tenemos para ofrecerte
    </h4>
    <a-row type="flex" justify="space-around">
      <a-col v-for="(item, key) in items" :key="key" :sm="18" :md="6">
        <ItemService :item="item" />
      </a-col>
    </a-row>
  </div>
</template>

<script>
import ItemService from '@/components/atoms/ItemService.vue'
export default {
  components: {
    ItemService
  },
  data () {
    return {
      items: [
        {
          img: '/utils/coctel.jpg',
          description: 'Todo tipo de cocteles',
          title: 'Coctel'
        },
        {
          img: '/utils/comida.jpg',
          description: 'Comida preparada por los mejores chef de la costa',
          title: 'Buffet'
        },
        {
          img: '/utils/piscina.jpg',
          description: 'Piscina con vista infinita al mar',
          title: 'Piscina'
        }
      ]
    }
  }
}
</script>
