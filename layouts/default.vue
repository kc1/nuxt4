<template>
<div>
<Menu/>
<!-- <Carousel/> -->
<nuxt/>
<!-- <Map/> -->
<Footer/>
</div>
</template>

<script>

// import VuetifyLogo from '~/components/VuetifyLogo.vue'
import Menu from '~/components/menu.vue'
import Footer from '~/components/footer.vue'
// import Carousel from '~/components/carousel.vue'
// import Map from '~/components/map.vue'

export default {
components: {
  // VuetifyLogo,
  // Map,
  // Carousel,
  Footer,
  Menu
}
}

</script>

<style>

</style>
