<template>
<div>
  <q-img src="http://xtrm.foxthemes.me/wp-content/uploads/2018/09/Group-27.png?id=3467">
      <div class="fit row no-wrap bg-transparent">
        <div class="Miles_for column no-wrap justify-center items-center content-start" >
          <span class="text-h2 text-bold">127</span>
          <span class="text-h6">Miles of Awesome Trails</span>
        </div>
        <div class="Miles_for column wrap justify-center items-center content-start">
          <span class="text-h2 text-bold">38</span>
          <span class="text-h6">Professional Instructors</span>
        </div>
        <div class="Miles_for column wrap justify-center items-center content-start">
          <span class="text-h2 text-bold">3.500</span>
          <span class="text-h6">Feets of Height Difference</span>
        </div>
        <div class="Miles_for column wrap justify-center items-center content-start">
          <span class="text-h2 text-bold">120K</span>
          <span class="text-h6">Riders Every Year</span>
        </div>

      </div>
  </q-img>
  <div>
    <div class="q-mt-xl q-ml-xl q-pt-xl">
      <span class="text-grey text-h6">PRICING</span><br>
      <span class="text-h4">Why Pay </span>
      <span class="bg-dark text-warning text-h4">More?</span>
    </div>
    <div style="width:100%;" class="row justify-around q-mt-xl q-pt-xl">
      <div class="for_more" v-for="more in mores" :key="more">
        <div class="q-mt-xl row wrap justify-around items-center content-start">
          <div>
            <span class="text-h2 text-bold">{{more.name}}<sup>{{more.name3}}</sup></span><br><br>
            <span class="text-h5">{{more.name2}}</span>
          </div>
            <q-btn class="bg-grey-4" unelevated disable>Monthly</q-btn>
        </div><br>
         <q-separator inset />
        <div class="column q-mt-xl q-ml-lg">
          <span class="text-h6"><q-icon color="warning" name="check"></q-icon> Unlimited Lift</span><br>
          <span class="text-h6"><q-icon name="check"></q-icon> Instructor’s Help</span><br>
          <span class="text-h6"><q-icon name="check"></q-icon> Free Hugs</span><br>
          <span class="text-h6"><q-icon name="check"></q-icon> Coffee & Cookies</span><br>
        </div>
        <q-btn outline size="20px" class="q-ml-lg">ORDER NOW</q-btn>
      </div>
    </div>


  </div>

<div style="height:100px;">

</div>

</div>
</template>
<script>
import { ref } from 'vue'
export default {
  setup () {
    return {
      slide: ref(1),
      autoplay: ref(true),
      mores:[
        {name3:'$',name:'80',name2:'Basic Plan'},
        {name3:'$',name:'100',name2:'Standard Plan'},
        {name3:'$',name:'120',name2:'Premium Plan'},
      ]
    }
  }
}
</script>
<style scoped>
.Miles_for{
  width:25%;
  height:100px;
  margin-top: 100px;
  margin-left: 20px;
}
.for_more{
  width: 28%;
  height: 550px;
  border: 2px solid rgb(182, 180, 180);
}

</style>
