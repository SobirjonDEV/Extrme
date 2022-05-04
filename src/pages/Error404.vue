<template>
  <div class="for_bac fullscreen  text-white text-center q-pa-md flex flex-center">
    <div>
      <div style="font-size: 30vh" class="fit column wrap justify-center items-center content-center">
        <img
        style="position: absolute; top:120px;"
        width="100"
        src="	https://xtrm.foxthemes.me/wp-content/uploads/2018/09/white-copy-9-1.png"
        alt="">
        <span >
          5555
        </span>
      </div>

      <div class=" ">
        <span class="text-bold text-h3">Huston, we have a</span>
        <span class="bg-orange-10 text-white text-bold text-h3"> problem!</span><br>
        <span class="text-p">The page which you looking for wouldn’t found, so keep calm and go home</span>
      </div>

      <q-btn
        class="q-mt-xl"
        outline
        color="white"
        text-color="white"
        unelevated
        to="/"
        label="Go Home"
        no-caps
        style="width:150px; height:50px;"
      />
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Error404'
})
</script>
<style scoped>
.for_bac{
  background-image: url(	https://xtrm.foxthemes.me/wp-content/uploads/2019/02/404.jpg);
}
</style>
