<template>
  <div class="villa__home">
    <div class="villa__home--secction">
      <a-row class="villa__home--section">
        <a-col>
          <logo />
          <img class="villa__home--branding" src="/utils/branding.jpg">
        </a-col>
        <a-col class="villa__home--row">
          <h4 class="villa__home--h4">
            POSADA
          </h4>
          <h1 class="villa__home--h1">
            Villa Paraiso
          </h1>
          <p class="villa__home--p">
            En un rinconcito de estado Sucre, a escasos 15 minutos de Puerto la Cruz, se encuentra Posada Villa Paraiso, vestida con los mejores calzados que brinda la naturaleza, montaña cumbre de Arapo y utilizando vestimenta del hermoso Parque Nacional Mochima.
          </p>
        </a-col>
        <a-col>
          <ButtonPrimary text="RESERVE YA" :click="handleClick" />
          <ButtonWhatsapp />
        </a-col>
      </a-row>
    </div>
    <div class="villa__home--section">
      <Services />
    </div>
    <div class="villa__home--section">
      <Events />
    </div>
    <div class="villa__home--section footer">
      <Footer />
    </div>
  </div>
</template>

<script>
import ButtonPrimary from '@/components/atoms/ButtonPrimary.vue'
import Logo from '@/components/atoms/Logo.vue'
import ButtonWhatsapp from '@/components/atoms/ButtonWhatsapp.vue'
import Services from '@/components/molecules/Services.vue'
import Events from '@/components/molecules/Events.vue'
import Footer from '@/components/molecules/Footer.vue'
export default {
  components: {
    ButtonPrimary,
    ButtonWhatsapp,
    Logo,
    Services,
    Events,
    Footer
  },
  methods: {
    handleClick () {
      console.log('action')
    }
  }
}
</script>
