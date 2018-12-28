<template>
<div>
<Menu/>
<Carousel/>
<Footer/>
</div>
</template>

<script>

import VuetifyLogo from '~/components/VuetifyLogo.vue'
import Menu from '~/components/menu.vue'
import Footer from '~/components/footer.vue'
import Carousel from '~/components/carousel.vue'

export default {
components: {
  VuetifyLogo,
  Carousel,
  Footer,
  Menu
}
}

</script>

<style>

</style>
