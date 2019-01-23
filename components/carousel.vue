<template>
<section>
 <v-card
    class="mx-auto"
    color="#26c6da"
    dark
    max-width="1200"
  >

  <v-carousel>
    <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.src"></v-carousel-item>
  </v-carousel>

</v-card>

</section>
</template>


<script>
  var cache = {};
  const images = require.context('../static/', false, /\.png$|\.jpg/);
  var imagesArray = Array.from(images.keys());
  // const images = ["./52lv.PNG", "./Capture1.PNG", "./maps.PNG"]
  console.log(images.keys());
  var constructed = [];
  function constructItems(fileNames, constructed) {
    fileNames.forEach(fileName => {
      constructed.push({
        'src': fileName.substr(1)
      })
    });
    return constructed;
  }
  console.log('items ');
  console.log(imagesArray);
  // At build-time cache will be populated with all required modules. 
  var res = constructItems(imagesArray, constructed);
  console.log(res);
  export default {
    data: function() {
      return {
        items: res
      };
    }
  };
  //     export default {
  //       data() {
  //         return {
  //           items: [{
  //               src: "/52lv.PNG"
  //             },
  //             {
  //               src: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg"
  //             },
  //             {
  //               src: "https://cdn.vuetifyjs.com/images/carousel/bird.jpg"
  //             },
  //             {
  //               src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg"
  //             }
  //           ]
  //         };
  //       }
  // };
</script>

