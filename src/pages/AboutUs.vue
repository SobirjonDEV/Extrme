<template>
  <div>
    <about-comp/>
    <about-comp-2/>
  <div class="for-orange_dark">
    <div class="for_bg-orange bg-orange-10  row no-wrap justify-around items-center content-start">
      <q-img width="140px" height="140px" src="https://xtrm.foxthemes.me/wp-content/uploads/2019/01/bitmap-1.png"/>
      <q-img width="200px" height="120px" src="https://xtrm.foxthemes.me/wp-content/uploads/2019/01/5.png"/>
      <q-img width="140px" height="140px" src="https://xtrm.foxthemes.me/wp-content/uploads/2019/01/bitm4ap.png"/>
      <q-img width="130px" height="150px" src="https://xtrm.foxthemes.me/wp-content/uploads/2019/01/10.png"/>
      <q-img width="140px" height="110px" src="https://xtrm.foxthemes.me/wp-content/uploads/2019/01/bit4map.png"/>
      <q-img width="120px" height="150px" src="https://xtrm.foxthemes.me/wp-content/uploads/2019/01/bitmfap.png"/>
    </div>
    <div class="for_bg-dark bg-dark"><br><br><br><br>
      <div class="for_margin">
        <span class="text-h5 text-white">newsletter</span><br><br>
        <span class="text-grey">A well-executed brand strategy affects all aspects of a business and is <br> connected to consumer needs & emotions.
        </span><br><br>
      <q-input class="for-input"  filled bottom-slots v-model="text" label="Your Email"  :dense="dense">
        <template v-slot:append>
          <q-icon
           name="arrow_upward"
           style=" position: absolute; right: 0px"
           @click="text = ''"
           class="cursor-pointer bg-orange-10 text-white " size="56px" />
        </template>
      </q-input>
      </div>
      <div><br><br>
        <span class="q-ml-xl q-pl-xl text-white ">© XTRM. All Right Reserved 2019.</span>
      </div>
    </div>
  </div>



  </div>
</template>
<script>
import AboutComp from 'src/components/AboutComp'
import AboutComp2 from 'src/components/AboutComp2'
export default {
  components: {
    AboutComp,
    AboutComp2
  },
  data() {
    return {

    }
  },
}
</script>
<style scoped>
.for_margin{
  margin-left: 170px;

}
.for_bg-orange{
  width: 100%;
  height:300px;
}
.for_bg-dark{
   width: 100%;
   height:350px;
}
.for-input{
  width: 450px;
  background-color: #fff;
  height: 56px;
}

</style>
