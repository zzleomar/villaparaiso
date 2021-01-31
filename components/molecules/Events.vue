<template>
  <div class="villa__events">
    <h4 class="villa__events--h4">
      Eventos
    </h4>
    <a-row type="flex" justify="space-around">
      <a-col v-for="(item, key) in items" :key="key" :sm="18" :md="6">
        <ItemEvent :item="item" />
      </a-col>
    </a-row>
  </div>
</template>

<script>
import ItemEvent from '@/components/atoms/ItemEvent.vue'
export default {
  components: {
    ItemEvent
  },
  data () {
    return {
      items: [
        {
          img: 'utils/carnavales.jpg',
          description: 'Ven y da el grito de carnaval aqui entre tragos y música',
          title: 'Carnaval'
        },
        {
          img: 'utils/party.jpg',
          description: 'En nuestras instalaciones nunca la pasaras mal',
          title: 'Pool party'
        },
        {
          img: 'utils/lugar.jpg',
          description: 'Reserva tu full day y creenos que volveras',
          title: 'Full day'
        }
      ]
    }
  }
}
</script>
