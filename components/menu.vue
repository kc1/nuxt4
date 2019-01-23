    <template>
      <v-toolbar color="indigo" dark>
        <v-toolbar-side-icon></v-toolbar-side-icon>
        <v-toolbar-title class="white--text">Land For Sale</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-toolbar-items class="hidden-sm-and-down">
           <v-btn flat v-for="action in toolbarActions" :key="action">{{action}}</v-btn>
                 <!-- <v-btn flat v-for="action in toolbarActions">{{action}}</v-btn> -->
          <!-- <v-btn flat>Link One</v-btn>
          <v-btn flat>Link Two</v-btn>
          <v-btn flat>Link Three</v-btn> -->
        </v-toolbar-items>
      </v-toolbar>
    </template>

  <script>

  // import toolbarActions from '~/store/store.js'

  //  export default {
  //   computed: {
  //     toolbarActions() {
  //             return this.$store.state.toolbarActions

  //             // return [ 'My project', 'Home', 'About', 'Contact' ]
  //     }
  //   }
  // } 
  export default {
    computed: {
  toolbarActions() {
      return this.$store.state.toolbar.toolbarActions  //look i added the name of the toolbar module

  }
 }
}
  </script>

  <style>

  </style>
