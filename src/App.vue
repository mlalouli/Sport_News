<template>
  <div >
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
          >
        </v-toolbar-title>
  <div class="d-flex justify-space-around">
    <v-btn>
      <img 
        alt="Scores" 
        data-src="/ls-web-assets/svgs/common/football-scores-4ca9dd32123cdc21863025c7beeb069a.svg" 
        loading="lazy" 
        width="20" 
        height="20" 
        decoding="async" 
        data-nimg="1" 
        src="https://www.livescore.com/ls-web-assets/svgs/common/football-scores-4ca9dd32123cdc21863025c7beeb069a.svg" 
        style="color: transparent;"
      >
      Scores
      
    </v-btn>

    <v-btn>
      <img 
        alt="Favourites" 
        data-src="/ls-web-assets/svgs/common/favourites-d308421de90923c9f7c0f8e0867e45d3.svg" 
        loading="lazy"
        width="20" 
        height="20" 
        decoding="async" 
        data-nimg="1" 
        src="https://www.livescore.com/ls-web-assets/svgs/common/favourites-d308421de90923c9f7c0f8e0867e45d3.svg" 
        style="color: transparent;"
      >
      Favourites
    </v-btn>

    <v-btn>
      <img 
        alt="News" 
        data-src="/ls-web-assets/svgs/common/news-article-active-9bb36e542cef2622d1897c5fba3657ea.svg" 
        loading="lazy" 
        width="20" 
        height="20" 
        decoding="async" 
        data-nimg="1" 
        src="https://www.livescore.com/ls-web-assets/svgs/common/news-article-active-9bb36e542cef2622d1897c5fba3657ea.svg" 
        style="color: transparent;"
      >
      <span style="color: #ff6b00;">
        News
      </span>
    </v-btn>

    <v-btn>
      <img 
        alt="Get the app" 
        data-src="/ls-web-assets/svgs/common/download-a627554318349f77bb4b3634e94b0205.svg" 
        loading="lazy" 
        width="20" 
        height="20" 
        decoding="async" 
        data-nimg="1" 
        src="https://www.livescore.com/ls-web-assets/svgs/common/download-a627554318349f77bb4b3634e94b0205.svg" 
        style="color: transparent;"
        >
      Get the app
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

      <v-main style="height: 1315px;">
        
  <v-card-text>

    <div style="background-color: red; width: 50%;margin-left: 25%;  ">      
  <v-sheet class="mx-auto" max-width="600">
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
  


    <v-carousel hide-delimiters  style="width: 80%;height: 30%; margin-left: 9%;">
      <v-carousel-item
      v-for="(item,i) in item"
      :key="i"
      :src="item.src"
      cover
      width="100%"
      
      > <div class="d-flex flex-column fill-height justify-center align-center text-white">
        
        <h3 class="Gt" data-testid="article-slide_title"  >Lescott: Who Id pick to help England win Euro 2024</h3>
      </div></v-carousel-item>
    </v-carousel>
  </div>
  
</v-card-text>
<div style="height: 100%;width: 50%;background-color: #ff6b00; margin-left: 25%;">
  
</div>
</v-main>
</v-layout>
<div style="height: 50%;width: 100%;background-color: red;"></div>
</v-card>
</div>
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
        item: [
          {
            src: 'https://uk1.sportal365images.com/process/smp-image-api/livescore.com/18032024/620b4100-40d2-4df3-a548-9d00d5d875a4.jpg?operations=fit(620:)&w=620&quality=100',
          },
          {
            src: 'https://uk1.sportal365images.com/process/smp-image-api/livescore.com/18032024/2c63e784-126f-4049-b7fc-3f902d97bd0c.jpg?operations=fit(620:)&w=620&quality=100',
          },
          {
            src: 'https://uk1.sportal365images.com/process/smp-image-api/livescore.com/18032024/7cd41289-670d-4946-a198-4692b729a20b.jpg?operations=fit(620:)&w=620&quality=100',
          },
        ],
        news: [
          'Lescott: Who Id pick to help England win Euro 2024',
          'fgijbnijfg',

          'fkvmofsmvo',
        ],
    }),
    

    watch: {
      group () {
        this.drawer = false
      },
    },
  }
</script>
