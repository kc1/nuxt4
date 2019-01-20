<template>
   <div>
     
       <!-- <Carousel/> -->
       <Two/>
       <Card/>
       <Panel/>
       <Three/>
       <Four/>
       </div> 
</template>

<script>
import Two from '~/components/section2.vue'
import Three from '~/components/section3.vue'
import Four from '~/components/section4.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'
import Menu from '~/components/menu.vue'
import Carousel from '~/components/carousel.vue'
import Panel from '~/components/detailSection.vue'
import Card from '~/components/detailCard.vue'


export default {

  components: {
    Two,
    Three,
    Four,
    Panel,
    Card,
    Carousel
  }

}
</script>

<style>

</style>


