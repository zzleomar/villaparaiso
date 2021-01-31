<template>
  <div class="villa__footer">
    <logo />
    <h4 class="villa__footer--h4">
      DIRECCIÓN
    </h4>
    <p class="villa__footer--p">
      Encuentranos a solo 15 minutos de Puerto La Cruz, Troncal 9, Cumbres de Guatamare 6001, Anzoátegui.
    </p>
    <ButtonRedes />
  </div>
</template>

<script>
import Logo from '@/components/atoms/Logo.vue'
import ButtonRedes from '@/components/atoms/ButtonRedes.vue'
export default {
  components: {
    Logo,
    ButtonRedes
  }
}
</script>
