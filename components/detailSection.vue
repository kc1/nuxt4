<template>
  <v-app id="inspire">
    <v-expansion-panel>
      <v-expansion-panel-content v-for="(item,i) in items" :key="i">
        <div slot="header">{{item.header}}</div>
        <v-card>
          <v-card-text>{{item.text}}</v-card-text>
        </v-card>
      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-app>
</template>

<script>
  //    <div id="base">
  //        Dividable double lot in downtown Windham, with city water, sewer and electricity hookups. The property is Zoned for multifamily.
  // Due to an error in valuation, you have an opportunity to buy this property at half price.
  // An identically sized and zoned adjacent property with a multi-family house is valued at over 200,000 with the land valued at over 45,000.
  // Additionally, plans for building a multi-family structure will be included with the sale.
  // Owner is leaving state, and wants quick sale. Serious offers only.
  // -
  //        </div> 
import * as data from '../static/info.json';

const word = data.name;

console.log(word); // output 'testing'


  export default {
    data() {
      return {
        panel: 'Sample panel',
        items: [{
            header: 'item 1',
            text: 'Lorem ipsum dolor sit amet, consectetur'
          },
          {
            header: 'item 2',
            text: 'sed do eiusmod tempor incididunt ut labore et'
          },
          {
            header: 'item 3',
            text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit,  dolore magna aliqua. Ut enim ad minim veniam,  commodo consequat.'
          },
          {
            header: 'item 4',
            text: 'quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea'
          },
        ]
      }
    }
  }
</script>

<style>

</style>
