<template>
  <div >
  <v-card>

 <!-- Nav-bar -->

    <v-layout>
      <!-- <v-system-bar color="deep-purple darken-3"></v-system-bar> -->

      <v-app-bar
        color="black"
        prominent
      >
        <v-app-bar-nav-icon variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

        <v-toolbar-title><img 
                    alt="livescore" 
                    fetchpriority="high" 
                    width="104" 
                    height="19" 
                    decoding="async" 
                    data-nimg="1" 
                    style="color: transparent;" 
                    src="https://www.livescore.com/ls-web-assets/svgs/common/livescore-logo-b3b211143dccd9e22d164701d32a390f.svg"
          >
        </v-toolbar-title>
<!-- top-bar -->
     <div class="menu d-flex justify-space-around">
        <TopBar />
     </div>
        <v-spacer></v-spacer>
        
        
       
      </v-app-bar>

      <v-navigation-drawer
        v-model="drawer"
        location="left"
        temporary
      >
        <v-list
          :items="items"
        ></v-list>
      </v-navigation-drawer>

      <v-main style="height: 1315px;">
        
  <v-card-text>

    <div style="background-color: #363535; width: 100%;margin-left: 0%;  ">      
  <v-sheet class=" mx-auto" max-width="600">
    <v-slide-group show-arrows>
      <v-slide-group-item
        v-slot="{ isSelected, toggle }"
        v-for="(slide, i) in slides"
        :key="i"
      >
        <v-btn
        :color="color[i]"
          class="ma-2"
          rounded
          @click="toggle"
        >
          <div class="d-flex fill-height justify-center align-center">
            <div class="text-h7">{{ slide }} </div>
          </div>
        </v-btn>
      </v-slide-group-item>
    </v-slide-group>
  </v-sheet>

   
    <div >
      <News />
    </div>


  </div>

  
  
</v-card-text>
</v-main>
</v-layout>

</v-card>
</div>
</template>

<script>
import News from './components/News.vue'
import TopBar from './components/TopBar.vue'
  export default {
    data: () => ({
      drawer: false,
      group: null,
      items: [
        {
          title: 'Settings',
          value: 'Settings',
        },
        {
          title: 'What is New?',
          value: 'What is New?',
        },
        {
          title: 'FAQ',
          value: 'FAQ',
        },
        {
          title: 'Contact',
          value: 'Contact',
        },
        {
          title: 'Advertise',
          value: 'Advertise',
        },
        {
          title: 'Mobile',
          value: 'Mobile',
        },
        {
          title: 'Privacy Notice',
          value: 'Privacy Notice',
        },
        {
          title: 'Language',
          value: 'Language',
        },
      ],
      color: [
          '#fdfdfd'
        ],
        slides: [
          'All',
          'Football',
          'Exclusives',
          'Transfer news',
          'Predictions',
          'Champions League',
          'Womens',
          'Other sport',
          'Match reports',
        ],
    }),
    

    watch: {
      group () {
        this.drawer = false
      },
    },
  }
</script>

