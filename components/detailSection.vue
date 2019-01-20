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
  import * as data from '../static/info.json';
  console.log(data); // output 'testing'
  console.log('djfhsjdfhs'); // output 'testing'
  var itemsArray = [];
  Object.keys(data.default).forEach(function(key) {
    // console.log(key, data[key]);
    itemsArray.push({
      header: key,
      text: data.default[key]
    });
  });
  // var jsonData = JSON.parse(data);
  console.log('hi there'); // output 'testing'
  console.log(itemsArray); // output 'testing'
  export default {
    data() {
      return {
        panel: 'Sample panel',
        items: itemsArray
     }
    }
  }
</script>

<style>

</style>
