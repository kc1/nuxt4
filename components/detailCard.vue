 <template>
  <v-card
    class="mx-auto"
    color="#26c6da"
    dark
    max-width="1200"
  >
    <v-card-title>
      <!-- <v-icon
        large
        left
      >
        mdi-twitter
      </v-icon> -->
      <!-- <span class="title font-weight-light">Twitter</span> -->
    </v-card-title>

    <v-card-text class="headline font-weight-bold">{{myData.Ad}}</v-card-text>

    <v-card-actions>
      <v-list-tile class="grow">
        <v-list-tile-avatar color="grey darken-3">
          <v-img
            class="elevation-6"
            src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
          ></v-img>
        </v-list-tile-avatar>

        <v-list-tile-content>
          <v-list-tile-title>Evan You</v-list-tile-title>
        </v-list-tile-content>

        <v-layout
          align-center
          justify-end
        >
          <v-icon class="mr-1">mdi-heart</v-icon>
          <span class="subheading mr-2">256</span>
          <span class="mr-1">·</span>
          <v-icon class="mr-1">mdi-share-variant</v-icon>
          <span class="subheading">45</span>
        </v-layout>
      </v-list-tile>
    </v-card-actions>
  </v-card>
</template>   

<script>
  import * as data from '../static/info.json';
  console.log(data); // output 'testing'
  console.log('detailCard'); // output 'testing'
  console.log(data); // output 'testing'
    //  text: data.default[key]
  console.log('hi there'); // output 'testing'
  // const myData = data.default;
 
export default {
data() {
      return {
        myData:data.default
     }

}
}

</script>


<style>

</style>
