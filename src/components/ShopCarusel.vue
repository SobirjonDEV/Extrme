<template >
  <div class="q-ma-lg q-mt-xl">
    <div class="q-mt-xl text-h3 q-ml-md">
       <span >Let’s Go</span>
       <span class="bg-black text-yellow">Shopping</span>
    </div>
    <div class="row q-mt-xl justify-between">
      <HomeCrusel :slides="slides11" />
      <HomeCrusel :slides="slides12"/>
      <HomeCrusel :slides="slides13"/>
      <HomeCrusel :slides="slides14"/>
      <HomeCrusel :slides="slides15"/>
    </div>
    <div class="row q-mt-xl">
      <HomeCrusel :slides="slides1" />
      <HomeCrusel :slides="slides2"/>
      <HomeCrusel :slides="slides3"/>
      <HomeCrusel :slides="slides4"/>
      <HomeCrusel :slides="slides5"/>

    </div>
  </div>
</template>
<script>
import HomeCrusel from '../components/HomeCrusel'
export default {
  components: { HomeCrusel },
  data() {
    return {
      slides1:[
        {name:1 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-37-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-31-1.png"},
        {name:3 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-28-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-35-1.png"},
        {name:5 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-34-1.png"},
      ],
      slides2:[
        {name: 1, src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-31-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-28-1.png"},
        {name:3 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-35-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-34-1.png"},
        {name:5 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-37-1.png"},
      ],
      slides3:[
        {name:1 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-28-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-35-1.png"},
        {name:3 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-34-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-37-1.png"},
        {name:5, src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-31-1.png"},
      ],
      slides4:[
        {name:1 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-35-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-34-1.png"},
        {name:3 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-37-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-31-1.png"},
        {name:5 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-28-1.png"},
      ],
      slides5:[
        {name:1 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-34-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-37-1.png"},
        {name:3 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-31-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-28-1.png"},
        {name:5 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-35-1.png"},
      ],
      slides11:[
        {name:1 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-33-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-36-1.png"},
        {name:3 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-32-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-29-1.png"},
        {name:5 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-30-1.png"},
      ],
      slides12:[
        {name: 1, src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-36-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-32-1.png"},
        {name:3 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-29-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-30-1.png"},
        {name:5 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-33-1.png"},
      ],
      slides13:[
        {name:1 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-32-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-29-1.png"},
        {name:3, src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-30-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-33-1.png"},
        {name:5 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-36-1.png"},
      ],
      slides14:[
        {name:1 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-29-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-30-1.png"},
        {name:3 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-33-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-36-1.png"},
        {name:5 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-32-1.png"},
      ],
      slides15:[
        {name:1, src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-30-1.png"},
        {name:2 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-33-1.png"},
        {name:3 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-36-1.png"},
        {name:4 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-32-1.png"},
        {name:5 , src:"  https://xtrm.foxthemes.me/wp-content/uploads/2018/09/group-29-1.png"},
      ],
    }
  },

}
</script>
<style >

</style>
