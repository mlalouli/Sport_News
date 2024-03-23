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

    <div style="background-color: #363535; width: 100%;margin-left: 0%;  ">      
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

   
    <div >
  
        <div class="Mi">
          <div class="kl ll" id="news-news-list-item-2024032222145404834">
              <a id="article-image-link-2024032222145404834" >
                <div class="hl" id="article-image-wrapper-2024032222145404834">
                  <img  
                    data-src="https://uk1.sportal365images.com/process/smp-image-api/livescore.com/22032024/14f56de9-b7bf-4437-b3cc-fd435f82e7e9.jpg?operations=fit(260:)&amp;w=260&amp;quality=100" loading="lazy" width="260" height="160" decoding="async" data-nimg="1" src="https://uk1.sportal365images.com/process/smp-image-api/livescore.com/22032024/14f56de9-b7bf-4437-b3cc-fd435f82e7e9.jpg?operations=fit(260:)&amp;w=260&amp;quality=100" style="color: transparent;">
                </div>
             </a>
          <div class="ol" id="article-item-content-2024032222145404834">
              <a class="ql" id="article-item-title-link-2024032222145404834" >
                <h2 class="ml" id="article-item-content-title-2024032222145404834">
                  Robertson admits Scots must improve at Euros after Netherlands collapse
                </h2>
              </a>
                <div class="pl" id="article-item-footer-2024032222145404834">
                    <div id="article-list-tags-2024032222145404834" class="Lq">
                      <a id="tag-link-Scotland" class="Mq" >
                        <span id="tag-label-Scotland">
                          <span>Scotland</span>
                        </span>
                      </a>
                      <a id="tag-link-Andrew Robertson" class="Mq">
                        <span id="tag-label-Andrew Robertson">
                        <span>Andrew Robertson</span>
                        </span>
                      </a>
                      <a id="tag-link-Netherlands" class="Mq" ><span id="tag-label-Netherlands">
                        <span>Netherlands</span>
                        </span>
                      </a>
                    </div>
                    <a class="rl" id="article-item-footer-link-2024032222145404834" >
                      <div class="tl" id="article-item-date-2024032222145404834">1 hour ago</div>
                    </a>
                </div>
            </div>
          </div></div>
        <div class="Mi">
          <div class="kl ll" id="news-news-list-item-2024032222145404834">
            <a id="article-image-link-2024032222145404834" >
              <div class="hl" id="article-image-wrapper-2024032222145404834">
                <img 
                  alt="Steve Clarke’s Scotland were hammered in Amsterdam (Joris Verwijst/PA)" id="article-item-image-2024032221513452165" 
                  data-src="https://image.assets.pressassociation.io/v2/image/production/65c751f471aba4367cd8fe40f3186c77Y29udGVudHNlYXJjaGFwaSwxNzExMjMwMTY4/2.75691725.jpg?rect=566,150,3202,1801&amp;ext=.jpg&amp;operations=fit(260:)&amp;w=260&amp;quality=100" loading="lazy" width="260" height="160" decoding="async" data-nimg="1" src="https://image.assets.pressassociation.io/v2/image/production/65c751f471aba4367cd8fe40f3186c77Y29udGVudHNlYXJjaGFwaSwxNzExMjMwMTY4/2.75691725.jpg?rect=566,150,3202,1801&amp;ext=.jpg&amp;operations=fit(260:)&amp;w=260&amp;quality=100" 
                  style="color: transparent;">
              </div>
            </a>
          <div class="ol" id="article-item-content-2024032222145404834">
              <a class="ql" id="article-item-title-link-2024032222145404834" >
                <h2 class="ml" id="article-item-content-title-2024032222145404834">
                  Netherlands 4-0 Scotland: Tartan Army crumble in Amsterdam
                </h2>
              </a>
                <div class="pl" id="article-item-footer-2024032222145404834">
                    <div id="article-list-tags-2024032222145404834" class="Lq">
                      <a id="tag-link-Scotland" class="Mq" >
                        <span id="tag-label-Scotland">
                          <span>Scotland</span>
                        </span>
                      </a>
                    <a id="tag-link-Andrew Robertson" class="Mq">
                      <span id="tag-label-Andrew Robertson">
                        <span>Andrew Robertson</span>
                      </span>
                    </a>
                    <a id="tag-link-Netherlands" class="Mq" ><span id="tag-label-Netherlands"><span>Netherlands</span></span></a></div><a class="rl" id="article-item-footer-link-2024032222145404834" ><div class="tl" id="article-item-date-2024032222145404834">1 hour ago</div>
                    </a>
                  </div>
            </div>
            </div></div>
        <div class="Mi">
          <div class="kl ll" id="news-news-list-item-2024032222145404834">
            <a id="article-image-link-2024032222145404834" >
              <div class="hl" id="article-image-wrapper-2024032222145404834">
                <img alt="Northern Ireland’s Jamie Reid celebrates his goal (Andreea Alexandru/AP)." id="article-item-image-2024032221513665000" data-src="https://content.assets.pressassociation.io/AP/2024/03/22/c49f3c03d1ad4d968a8a2f57a206f920.jpg?rect=0,137,5044,2837&amp;ext=.jpg&amp;operations=fit(260:)&amp;w=260&amp;quality=100" loading="lazy" width="260" height="160" decoding="async" data-nimg="1" src="https://content.assets.pressassociation.io/AP/2024/03/22/c49f3c03d1ad4d968a8a2f57a206f920.jpg?rect=0,137,5044,2837&amp;ext=.jpg&amp;operations=fit(260:)&amp;w=260&amp;quality=100" style="color: transparent;"
                />
              </div>
            </a>
          <div class="ol" id="article-item-content-2024032222145404834">
              <a class="ql" id="article-item-title-link-2024032222145404834" >
                <h2 class="ml" id="article-item-content-title-2024032222145404834">
                  Romania 1-1 Northern Ireland: Reid’s debut goal earns encouraging away draw
                </h2>
              </a>
                <div class="pl" id="article-item-footer-2024032222145404834">
                    <div id="article-list-tags-2024032222145404834" class="Lq">
                      <a id="tag-link-Scotland" class="Mq" >
                        <span id="tag-label-Scotland">
                          <span>Scotland</span>
                        </span>
                      </a>
                    <a id="tag-link-Andrew Robertson" class="Mq">
                      <span id="tag-label-Andrew Robertson">
                        <span>Andrew Robertson</span>
                      </span>
                    </a>
                    <a id="tag-link-Netherlands" class="Mq" ><span id="tag-label-Netherlands"><span>Netherlands</span></span></a></div><a class="rl" id="article-item-footer-link-2024032222145404834" ><div class="tl" id="article-item-date-2024032222145404834">1 hour ago</div>
                    </a>
                  </div>
            </div>
            </div></div>
        <div class="Mi">
          <div class="kl ll" id="news-news-list-item-2024032222145404834">
            <a id="article-image-link-2024032222145404834" >
              <div class="hl" id="article-image-wrapper-2024032222145404834">
                <img alt="Paul Warne's Derby have won their last four games, keeping three clean sheets, to take a grip of second place" id="article-item-image-2024032212390729300" data-src="https://uk1.sportal365images.com/process/smp-image-api/livescore.com/22032024/9b5b8e91-f23e-4c07-bb07-1c73cf60ff31.jpg?operations=fit(260:)&amp;w=260&amp;quality=100" loading="lazy" width="260" height="160" decoding="async" data-nimg="1" src="https://uk1.sportal365images.com/process/smp-image-api/livescore.com/22032024/9b5b8e91-f23e-4c07-bb07-1c73cf60ff31.jpg?operations=fit(260:)&amp;w=260&amp;quality=100" 
                  style="color: transparent;"
                />
              </div>
            </a>
          <div class="ol" id="article-item-content-2024032222145404834">
              <a class="ql" id="article-item-title-link-2024032222145404834" >
                <h2 class="ml" id="article-item-content-title-2024032222145404834">
                  Saturday EFL predictions: Four teams to follow in the EFL
                </h2>
              </a>
                <div class="pl" id="article-item-footer-2024032222145404834">
                    <div id="article-list-tags-2024032222145404834" class="Lq">
                      <a id="tag-link-Scotland" class="Mq" >
                        <span id="tag-label-Scotland">
                          <span>Scotland</span>
                        </span>
                      </a>
                    <a id="tag-link-Andrew Robertson" class="Mq">
                      <span id="tag-label-Andrew Robertson">
                        <span>Andrew Robertson</span>
                      </span>
                    </a>
                    <a id="tag-link-Netherlands" class="Mq" ><span id="tag-label-Netherlands"><span>Netherlands</span></span></a></div><a class="rl" id="article-item-footer-link-2024032222145404834" ><div class="tl" id="article-item-date-2024032222145404834">1 hour ago</div>
                    </a>
                  </div>
            </div></div></div>
        <div class="Mi">
          <div class="kl ll" id="news-news-list-item-2024032222145404834">
            <a id="article-image-link-2024032222145404834" >
              <div class="hl" id="article-image-wrapper-2024032222145404834">
                <img alt="Neco Williams (second left) celebrates after scoring Wales’ second goal in their 4-1 Euro 2024 play-off victory over Finland (Nick Potts/PA)" id="article-item-image-2024032121553630141" data-src="https://image.assets.pressassociation.io/v2/image/production/ab63348f615b573478e750755dc1d244Y29udGVudHNlYXJjaGFwaSwxNzExMTQzMzEw/2.75683709.jpg?rect=0,238,5432,3055&amp;ext=.jpg&amp;operations=fit(260:)&amp;w=260&amp;quality=100" loading="lazy" width="260" height="160" decoding="async" data-nimg="1" src="https://image.assets.pressassociation.io/v2/image/production/ab63348f615b573478e750755dc1d244Y29udGVudHNlYXJjaGFwaSwxNzExMTQzMzEw/2.75683709.jpg?rect=0,238,5432,3055&amp;ext=.jpg&amp;operations=fit(260:)&amp;w=260&amp;quality=100" style="color: transparent;"
                />
              </div>
            </a>
          <div class="ol" id="article-item-content-2024032222145404834">
              <a class="ql" id="article-item-title-link-2024032222145404834" >
                <h2 class="ml" id="article-item-content-title-2024032222145404834">
                  Wales 4-1 Finland: Dragons set up Poland showdown for Euros spot
                </h2>
              </a>
                <div class="pl" id="article-item-footer-2024032222145404834">
                    <div id="article-list-tags-2024032222145404834" class="Lq">
                      <a id="tag-link-Scotland" class="Mq" >
                        <span id="tag-label-Scotland">
                          <span>Scotland</span>
                        </span>
                      </a>
                    <a id="tag-link-Andrew Robertson" class="Mq">
                      <span id="tag-label-Andrew Robertson">
                        <span>Andrew Robertson</span>
                      </span>
                    </a>
                    <a id="tag-link-Netherlands" class="Mq" ><span id="tag-label-Netherlands"><span>Netherlands</span></span></a></div><a class="rl" id="article-item-footer-link-2024032222145404834" ><div class="tl" id="article-item-date-2024032222145404834">1 hour ago</div>
                    </a>
                  </div>
            </div>
            </div></div>
        <div class="Mi">
                  <div class="kl ll" id="news-news-list-item-2024032222145404834">
                    <a id="article-image-link-2024032222145404834" >
                      <div class="hl" id="article-image-wrapper-2024032222145404834">
                        <img alt="Gareth Southgate's England are on a 10-match unbeaten run" id="article-item-image-2024032115272722222" data-src="https://uk1.sportal365images.com/process/smp-image-api/livescore.com/21032024/963427c5-4e7e-4de1-9f5b-c25948ee5d6b.jpg?operations=fit(260:)&amp;w=260&amp;quality=100" loading="lazy" width="260" height="160" decoding="async" data-nimg="1" src="https://uk1.sportal365images.com/process/smp-image-api/livescore.com/21032024/963427c5-4e7e-4de1-9f5b-c25948ee5d6b.jpg?operations=fit(260:)&amp;w=260&amp;quality=100" style="color: transparent;"
                        />
                      </div>
                    </a>
                  <div class="ol" id="article-item-content-2024032222145404834">
                      <a class="ql" id="article-item-title-link-2024032222145404834" >
                        <h2 class="ml" id="article-item-content-title-2024032222145404834">
                          England vs Brazil predictions: Glamour friendly to end all-square
                        </h2>
                      </a>
                        <div class="pl" id="article-item-footer-2024032222145404834">
                            <div id="article-list-tags-2024032222145404834" class="Lq">
                              <a id="tag-link-Scotland" class="Mq" >
                                <span id="tag-label-Scotland">
                                  <span>Scotland</span>
                                </span>
                              </a>
                            <a id="tag-link-Andrew Robertson" class="Mq">
                              <span id="tag-label-Andrew Robertson">
                                <span>Andrew Robertson</span>
                              </span>
                            </a>
                            <a id="tag-link-Netherlands" class="Mq" ><span id="tag-label-Netherlands"><span>Netherlands</span></span></a></div><a class="rl" id="article-item-footer-link-2024032222145404834" ><div class="tl" id="article-item-date-2024032222145404834">1 hour ago</div>
                            </a>
                          </div>
                    </div></div></div>


    </div>
  </div>
  
</v-card-text>

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
          {
            comment: 'Lescott: Who Id pick to help England win Euro 2024'
          },
          {
            comment: 'fgijbnijfg',
          },
          {
            comment: 'fkvmofsmvo',
          }
          

          
        ],
    }),
    

    watch: {
      group () {
        this.drawer = false
      },
    },
  }
</script>

