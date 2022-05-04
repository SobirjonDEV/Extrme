<template>
  <q-layout view="hhh lpR fff">
    <q-header bordered class="transparent text-white" style="height:100px;">
      <q-toolbar>
        <q-toolbar-title>
        <div class="fit row no-wrap justify-center items-center q-mt-md">
          <div class="row no-wrap justify-center items-center q-mt-md">
            <span style="whith:10%;" class=" q-mr-xl q-pr-xl text-bold text-h4" >
              <img src="	https://xtrm.foxthemes.me/wp-content/uploads/2018/09/white.png">
              </span>
              <a target="blanc"  href="https://preview.themeforest.net/item/xtrm-extreme-sports-wordpress-theme/full_screen_preview/23423423?_ga=2.160074877.1141608953.1649333502-489852383.1649243492">xtrm</a>
              <div class="" v-for="select in selects" :key="select">
                <q-btn-dropdown  color="transparent" unelevated :label="select.label"><q-list>
                  <q-item  :to="select.to"  clickable v-close-popup @click="onItemClick">
                    <q-item-section>
                      <q-item-label>{{select.name}}</q-item-label>
                    </q-item-section>
                  </q-item>
                   <q-item  clickable v-close-popup @click="onItemClick">
                    <q-item-section>
                      <q-item-label>{{select.fname}}</q-item-label>
                    </q-item-section>
                  </q-item>
                   <q-item  clickable v-close-popup @click="onItemClick">
                    <q-item-section>
                      <q-item-label>{{select.namef}}</q-item-label>
                    </q-item-section>
                  </q-item>
                </q-list>
              </q-btn-dropdown>
            </div>

          <q-icon name="search" size="30PX" class="q-ml-xl q-pl-lg" />
          <q-icon name="shopping_bag " size="30px"  class="q-ml-md"/>
          </div>
        </div>
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />

    </q-page-container>



  </q-layout>
</template>
<script>
import { ref } from 'vue'
export default {
  data() {
    return {
      model: ref(null),
      options: [
        'Google', 'Facebook', 'Twitter', 'Apple', 'Oracle'
      ],
       onItemClick () {
        // console.log('Clicked on an Item')
      },
        selects:[
        {name:'404',to:'/:catchAll(.*)*', label:'home'},
        {name:'AboutUs',to:'/aboutus',label:'pages'},
        {name:'Photos', label:'showcases'},
        {name:'Photos', label:'blog',},
        {name:'Photos', label:'shop'},
        {name:'Photos', label:'pricing'},
        {name:'Photos', label:'contact us'},
      ],
    }
  },
}
</script>
