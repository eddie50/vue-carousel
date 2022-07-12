<template>
  <Carousel 
    :slides="slides" 
    controls 
    indicators 
    :interval="3000"
    :width="1000"
    :height="450"
  />
</template>

<script>
import Carousel from './components/carousel/Carousel.vue'
export default {
  components:{Carousel},
  data(){
    return{
      slides:[
      "https://picsum.photos/id/1032/1000/450",
      "https://picsum.photos/id/1033/1000/450",
      "https://picsum.photos/id/1037/1000/450",
      "https://picsum.photos/id/1035/1000/450",
      "https://picsum.photos/id/1036/1000/450",
    
    ]
    }
    
  }
}

</script>


