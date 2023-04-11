<template>
    <div>
        <vue-flux
        :options="fluxOptions"
        :images="fluxImages"
        :transitions="fluxTransitions"
        ref="slider" >
           <flux-pagination slot="pagination"></flux-pagination>
     </vue-flux>

    </div>
    
</template>

<script>
   import { VueFlux, FluxPagination, Transitions } from 'vue-flux';

export default {
   components: {
      VueFlux,
      FluxPagination
   },

   data: () => ({
      fluxOptions: {
         autoplay: true,
         height: "590px",
      },
      fluxImages: [ 'https://www.dharankitchen.com/img/slide2.jpg','https://www.dharankitchen.com/img/slide3.jpg', 'https://www.dharankitchen.com/img/slide1.jpg', ],
      fluxTransitions: {
         transitionBook: Transitions.transitionBook
      }
   })
}
</script>

<style scoped>


</style>