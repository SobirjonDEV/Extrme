<template>
  <div>
    <about-comp/>
    <div class="for_7one fit row wrap justify-center items-center content-start">
      <div class=" fit row wrap justify-end items-center q-mr-xl">
            <q-img
              v-for="img of imgs" :key="img"
              :class="img.class"
              :width="img.width"
              :height="img.height"
              :src="img.src">
              <div :class="img.calsstext">
                <span class="text-h6 text-white">About Gallery</span><br>
                <span class="text-h5 text-bold text-white">{{img.text}}</span>
              </div>
            </q-img>
          </div>
    </div>
    <div>
      <div class="for_avatar">
        <q-img src="	https://xtrm.foxthemes.me/wp-content/uploads/2019/01/group-15.jpg">
          <div class="for_content fit row wrap justify-around items-center content-center">
            <q-icon class="for_content" name="fab fa-instagram"></q-icon>
            <q-icon class="for_content" name="fab fa-facebook-square"></q-icon>
            <q-icon class="for_content" name="fab fa-twitter"></q-icon>
          </div>
        </q-img>
      </div>
    </div>

  </div>
</template>
<script>
import AboutComp from 'src/components/AboutComp'
export default {
  components: {
    AboutComp
  },
  data() {
    return {
      imgs:[
           {src:'https://xtrm.foxthemes.me/wp-content/uploads/2019/01/group-32-copy-2.jpg',
        text:'Endless Falling',
        calsstext:'for_text1 bg-transparent',
        width:"320px",
        height:'500px',
        class:'q-ml-lg'
        },
           {src:'https://avatars.mds.yandex.net/i?id=81c1b80185bc74f6de3de872515bef86-5884528-images-thumbs&n=13',
        text:'Endless Falling',
        calsstext:'for_text2 bg-transparent',
        width:"320px",
        height:'550px',
        class:'q-ml-lg q-mt-xl '
        },
           {src:'https://xtrm.foxthemes.me/wp-content/uploads/2019/01/group-32-copy-2.jpg',
        text:'Endless Falling',
        calsstext:'for_text3 bg-transparent',
        width:"320px",
        height:'400px',
        class:'for_freefal q-ml-lg '
        },
           {src:'https://xtrm.foxthemes.me/wp-content/uploads/2019/01/group-32-copy-2.jpg',
        text:'Endless Falling',
        calsstext:'for_text4 bg-transparent',
        width:"320px",
        height:'500px',
        class:'for_yellowboard q-ml-lg q-mt-lg'
        },
           {src:'https://xtrm.foxthemes.me/wp-content/uploads/2019/01/group-32-copy-2.jpg',
        text:'Endless Falling',
        calsstext:'for_text5 bg-transparent',
        width:"320px",
        height:'450px',
        class:'q-ml-lg q-mt-lg'
        },
           {src:'https://xtrm.foxthemes.me/wp-content/uploads/2019/01/group-32-copy-2.jpg',
        text:'Endless Falling',
        calsstext:'for_text6 bg-transparent',
        width:"320px",
        height:'280px',
        class:'for_newbikes q-ml-lg'
        },
            {src:'https://xtrm.foxthemes.me/wp-content/uploads/2019/01/group-32-copy-2.jpg',
        text:'Endless Falling',
        calsstext:'for_text7 bg-transparent',
        width:"320px",
        height:'300px',
        class:'for_goinghome q-ml-lg q-mb-lg'
        },



      ]
    }
  },
}
</script>
<style scoped>

.for_content{
  border-radius: 50%;
  background: transparent;
  color: white;
}
.for_content:hover{
  background: #f56923b9;
  border-radius: 50%;
  color: rgb(255, 255, 255);
  font-size: 30px;
}
.for_avatar{
  width:200px;
  height:200px;
  border-radius: 50%;
}
.for_goinghome{
  margin-top: -300px;
}
.for_freefal{
  margin-top: -100px;
}
.for_newbikes{
  margin-top: -450px;
}
.for_yellowboard{
  margin-top: -30px;
}
.for_7one{
  margin-left: -110px;
  margin-top: -190px;
}
.for_text1{
  margin-top:125%;
}
.for_text2{
  margin-top:140%;
}
.for_text3{
  margin-top:120%;
}
.for_text4{
  margin-top:125%;
}
.for_text5{
  margin-top:110%;
}
.for_text6{
  margin-top:55%;
}
.for_text7{
  margin-top:65%;
}



</style>
