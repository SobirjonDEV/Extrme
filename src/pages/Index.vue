<template>
<div>
  <!-- Navbardan Night Wolf karuslegacha -->
<home-comp/>
  <!--  Night Wolf karuslel dan shop gacha   -->
<home-comp-2/>
  <!--  Shop  -->
<shop-carusel/>
<!--  Shop dan  120K   gacha -->
<home-more/>
<!-- 120k dan  gacha -->


<div>
  <q-img src="http://xtrm.foxthemes.me/wp-content/uploads/2018/09/news.png?id=3395">
    <div class="bg-transparent fit row no-wrap justify-around items-center content-around">
      <span class="text-h4 text-bold">Want You Get a Week of Riding For Free?</span>
      <q-btn class="Free_btn bg-warning text-dark">I WANT IT </q-btn>
    </div>
  </q-img>
</div>
<div>
  <div class="q-ml-xl q-mt-xl q-pl-xl">
    <span class="text-h6 q-ml-xl text-grey">BLOG</span><br><br>
    <span class="text-h3 q-ml-xl">Our Latest</span>
    <span class="text-h3 bg-dark text-warning">News</span>
  </div>
  <div class="fit row no-wrap justify-around items-center content-start q-mt-xl">
    <q-card class="my-card" v-for="card in cards" :key="card">
      <img :src="card.img">
      <div class="quti bg-warning text-center text-bold text-dark q-ml-lg ">
        {{card.quti}}
      </div>

      <q-card-section>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-h6">by John Doe</div>
        <div class="text-p q-mt-xl ">4 year ago</div>
      </q-card-section>

    </q-card>
  </div>
  <div>
    <div class="for_new">
      <span class="text-h6">newsletter</span><br><br>
      <span class="text-p">A well-executed brand strategy affects all aspects of a business and is connected to consumer needs & emotions.</span>
      <q-input class="q-mt-xl" filled bottom-slots v-model="text" label="Your-Email"  >
          <template v-slot:append>
            <q-icon v-if="text !== ''"  @click="text = ''" class="cursor-pointer" />
          </template>
          <template v-slot:after>
            <q-btn class="bg-warning fit " size="20px"  dense flat icon="arrow_upward" />
          </template>
      </q-input><br><br><br><br><br><br>
      <div class="text-h6 q-mr-xl  row wrap justify-around items-start content-start" style="position: absolute; left:7%;">
        © XTRM. All Right Reserved 2019.
        <div class="icon2 row justify-around ">
          <div class="icon bg-dark text-center text-white">T</div>
          <div class="icon bg-dark text-center text-white">F</div>
          <div class="icon bg-dark text-center text-white">I</div>
          <div class="icon bg-dark text-center text-white">G</div>
          <div class="icon bg-dark text-center text-white">P</div>

        </div>
      </div>
    </div>
  </div>
</div>

</div>
</template>
<script>
import { ref } from 'vue'
import HomeComp from '../components/HomeComp'
import HomeComp2 from '../components/HomeComp2'
import ShopCarusel from 'src/components/ShopCarusel.vue'
import HomeMore from '../components/Home.More'
export default {
   components:{
      HomeComp,
      HomeComp2,
      ShopCarusel,
      HomeMore
  },
  setup () {
    return {
      cards:[
        {img:'https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-16.jpg',quti:'NEWS'},
        {img:'https://xtrm.foxthemes.me/wp-content/uploads/2018/09/grou3p-16.jpg',quti:'Events'},
        {img:'https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group2-16.jpg',quti:'TrailReviews'},
        {img:'https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-6.jpg',quti:'NEWS'}
      ]
    }
  }
}
</script>
<style scoped>
.Free_btn{
  width:140px;
  height:50px;
}
.my-card{
  width:20%;
  height:350px;
  transition: 0.5s;
}
.my-card:hover{
  width:20%;
  height:350px;
  margin-top: -30px;
  box-shadow: 30px;
  transition: 0.1s;
}
.quti{
  position: absolute;
  top: 44%;
}
.for_new{
  width:35%;
  margin-left: 200px;
  margin-top: 200px;
}
.icon{
  width:40px;
  height:40px;
  margin-left: 10px;
}
.icon2{
  margin-left: 500px;
}
</style>
