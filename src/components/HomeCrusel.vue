  <template>
    <div>
      <q-carousel
        animated
        v-model="slide"
        transition-prev="slide-right"
        transition-next="slide-left"
        infinite
        autoplay="true"
        style="width:255px; height:550px"

      >
        <q-carousel-slide v-for="(slide, index) in slides" :key="index" :name="slide.name" class="carousel">
          <div  style="width:235px" class=" carousel-slide row justify-center">
            <div class="carousel-slide-img">
              <img  :src="slide.src" />
            </div>
            <div style="width:240px" class="q-ml-sm q-mt-lg">
              <span class="text-h5">Snowboord</span><br><br>
              <span class="text-h6 text-grey-7"> <del>$386.00</del>$320.00</span>
            </div>
          </div>
          <div class=" text1"><span style="padding:4px" class="bg-yellow "> Sn Equpiment</span></div>
          <div class=" text2"> <span class="bg-black q-pa-sm text-white">SALE</span></div>
        </q-carousel-slide>
      </q-carousel>
    </div>
</template>

<script>
import { ref } from 'vue'

export default {
  name:"IndexShopCarousel",
  props:["slides"],
  setup () {
    return {
      slide: ref(1)
    }
  }
}
</script>
<style scoped>
  .carousel{
    position: relative;
  }
  .carousel-slide{
    position: absolute;
  }
  .carousel-slide-img{
    width: 220px;
    height: 400px;
    border: 1px solid rgb(217, 216, 216)  ;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .text1{
    position:absolute;
    top: 40px;
    left: 20px;
  }
  .text2{
    position:absolute;
    top: 40px;
    left: 205px;
  }
</style>
