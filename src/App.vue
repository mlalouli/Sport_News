<template>
  <v-card>
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
                ></v-toolbar-title>
                <div class="d-flex justify-space-around">
    <v-btn>
      Start
      
    </v-btn>

    <v-btn>
      End
    </v-btn>

    <v-btn>
      Top
    </v-btn>

    <v-btn>
      Bottom
    </v-btn>
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

      <v-main style="height: 500px;">
        <v-card-text>


          <v-carousel
    height="100"
    color="black"
    hide-delimiters
  >
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
      <v-sheet
        height="100%"
      >
        <div class="d-flex fill-height justify-center align-center">
          <div class="text-h2">
            {{ slide }} Slide
          </div>
        </div>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>


        </v-card-text>
      </v-main>
    </v-layout>
  </v-card>
</template>

<script>

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
    }),
    

    watch: {
      group () {
        this.drawer = false
      },
    },
    data () {
      return {
        slides: [
          'First',
          'Second',
          'Third',
          'Fourth',
          'Fifth',
        ],
      }
    },
  }
</script>
