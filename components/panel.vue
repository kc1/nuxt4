  <template>
      <!-- <v-layout align-start > -->

      <!-- <v-layout align-start justify-center row fill-height> -->
      <v-container row fill-height justify-center style="max-width: 1200px"  >
                <!-- <v-layout row justify-space-around> -->

          <v-flex  >
            <v-expansion-panel  >
              <v-expansion-panel-content  v-for="(item,i) in items" :key="i" style="background:#26c6da;color:white">
                <div slot="header" class="headline font-weight-bold">{{item.header}}</div>
                <v-card >
                  <v-card-text class="headline font-weight-bold">{{item.text}}</v-card-text>
                </v-card>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-flex>
      </v-container>
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
