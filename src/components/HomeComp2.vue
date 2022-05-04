<template lang="">
  <div>
    <q-img class="q-mt-xl"
 src="http://xtrm.foxthemes.me/wp-content/uploads/2018/09/Group-38.png?id=3393">
<div class="q-pa-md bg-transparent" style="width:100%; height:100vh;">
    <q-carousel
      v-model="slide"
      swipeable
      animated
      padding
      arrows
      navigation
      navigation-icon="radio_button_unchecked"
      height="300px"
      class="bg-transparent text-white rounded-borders"
      style="margin-top:150px; height:70vh;"
    >
      <q-carousel-slide name="style" class="text-center ">
        <q-scroll-area class="fit">
          <span class="text-bold">TESTIMONIALS</span><br>
          <span class="text-h4 text-bold">Our Riders Said About Us</span>
          <div class="rating text-warning text-h5 q-mt-xl">
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
          </div>
          <div class="q-mt-md text-h5 text-bold">
            {{ lorem }}
          </div>
          <div class="q-mt-md text-h5 text-bold">
            Lorem ipsum dolor sit amet
          </div>
          <div style="width:20%; height:70px; margin-left:40%;" class=" row q-mt-lg">
            <img src="https://xtrm.foxthemes.me/wp-content/uploads/2018/09/Group-13.png">
            <div class="q-ml-sm q-mt-sm">
              <span class="text-h6 q-ml-md">Night Wolf</span><br>
              <span class="q-mr-lg">Pro Rider</span>
            </div>
          </div>
        </q-scroll-area>
      </q-carousel-slide>

      <q-carousel-slide name="tv" class="text-center">
        <q-scroll-area class="fit">
         <span class="text-bold">TESTIMONIALS</span><br>
          <span class="text-h4 text-bold">Our Riders Said About Us</span>
          <div class="rating text-warning text-h5 q-mt-xl">
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
          </div>
          <div class="q-mt-md text-h5 text-bold">
            {{ lorem }}
          </div>
          <div class="q-mt-md text-h5 text-bold">
            Lorem ipsum dolor sit amet
          </div>
          <div style="width:20%; height:70px; margin-left:40%;" class=" row q-mt-lg">
            <img src="https://xtrm.foxthemes.me/wp-content/uploads/2018/09/Group-13.png">
            <div class="q-ml-sm q-mt-sm">
              <span class="text-h6 q-ml-md">Night Wolf</span><br>
              <span class="q-mr-lg">Pro Rider</span>
            </div>
          </div>
        </q-scroll-area>
      </q-carousel-slide>

      <q-carousel-slide name="layers" class="text-center">
        <q-scroll-area class="fit">
          <span class="text-bold">TESTIMONIALS</span><br>
          <span class="text-h4 text-bold">Our Riders Said About Us</span>
          <div class="rating text-warning text-h5 q-mt-xl">
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
            <q-icon name="star"></q-icon>
          </div>
          <div class="q-mt-md text-h5 text-bold">
            {{ lorem }}
          </div>
          <div class="q-mt-md text-h5 text-bold">
            Lorem ipsum dolor sit amet
          </div>
          <div style="width:20%; height:70px; margin-left:40%;" class=" row q-mt-lg">
            <img src="https://xtrm.foxthemes.me/wp-content/uploads/2018/09/Group-13.png">
            <div class="q-ml-sm q-mt-sm">
              <span class="text-h6 q-ml-md">Night Wolf</span><br>
              <span class="q-mr-lg">Pro Rider</span>
            </div>
          </div>
        </q-scroll-area>
      </q-carousel-slide>
    </q-carousel>
  </div>
</q-img>
  </div>
</template>
<script>
import { ref } from 'vue'

export default {
  data() {
    return {
      slide: ref(1),
      lorem: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. ',

    }
  },
}
</script>
<style lang="">

</style>
