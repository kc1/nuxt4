<template>
          <section>
        <v-parallax src="assets/hero.jpeg" height="600">
          <v-layout
            column
            align-center
            justify-center
            class="white--text"
          >
            <img src="assets/vuetify.png" alt="Vuetify.js" height="200">
            <h1 class="white--text mb-2 display-1 text-xs-center">Parallax Template</h1>
            <div class="subheading mb-3 text-xs-center">Powered by Vuetify</div>
            <v-btn
              class="blue lighten-2 mt-5"
              dark
              large
              href="/pre-made-themes"
            >
              Get Started
            </v-btn>
          </v-layout>
        </v-parallax>
      </section>


</template>

<script>
  import * as data from '../static/info.json';
  console.log(data); // output 'testing'
  console.log('djfhsjdfhs'); // output 'testing'
    //  text: data.default[key]
  console.log('hi there'); // output 'testing'
 
export default {

}
</script>

<style>

</style>
