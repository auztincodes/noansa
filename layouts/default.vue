<template>
  <v-app>
    <div class="premium-container">
      <v-img class="coffee-image" :src="require('../assets/images/coffee-bean-spill.png')">
        <v-container>
          <v-toolbar flat color="transparent">
            <v-toolbar-title>NOANSA</v-toolbar-title>
            <div class="flex-grow-1"></div>

            <v-toolbar-items class="hidden-sm-and-down nav-item">
              <v-btn text>SHOP</v-btn>
              <v-btn text>WHOLESALE</v-btn>
              <v-btn text>LOCATIONS</v-btn>
              <v-btn text>OUR STORY</v-btn>
              <v-btn icon>
                <v-icon>mdi-magnify</v-icon>
              </v-btn>
              <v-btn icon>
                <v-icon>mdi mdi-account-circle</v-icon>
              </v-btn>
            </v-toolbar-items>
            <v-toolbar-items
              @click.stop="drawer = !drawer"
              class="nav-item hidden-md-and-up hidden-lg-and-up"
            >
              <v-btn icon>
                <v-icon>mdi-menu</v-icon>
              </v-btn>
            </v-toolbar-items>
          </v-toolbar>
          <!-- <v-tool-bar-items class="hidden-md-and-up nav-item">
        <v-btn color="pink" dark @click.stop="drawer = !drawer">Toggle</v-btn>
          </v-tool-bar-items>-->
          <v-navigation-drawer app v-model="drawer" right>
            <v-list-item>
              <v-list-item-content>
                <v-list-item-title>Menu</v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-divider></v-divider>

            <v-list dense>
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title>
                    <v-btn text>SHOP</v-btn>
                  </v-list-item-title>
                  <v-list-item-title>
                    <v-btn text>WHOLESALE</v-btn>
                  </v-list-item-title>
                  <v-list-item-title>
                    <v-btn text>LOCATIONS</v-btn>
                  </v-list-item-title>
                  <v-list-item-title>
                    <v-btn text>OUR STORY</v-btn>
                  </v-list-item-title>
                  <v-list-item-title>
                    <v-btn text>
                      <v-icon>mdi-magnify</v-icon>
                    </v-btn>
                  </v-list-item-title>
                  <v-list-item-title>
                    <v-btn text>
                      <v-icon>mdi mdi-account-circle</v-icon>
                    </v-btn>
                  </v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list>
          </v-navigation-drawer>
          <v-row no-gutters class="entry-fold">
            <v-flex md6 class="entry-fold-col">
              <p>PREMIUN COFFEE</p>
              <h4>A cup of coffee is one of the most important, simple pleasures in life.</h4>
              <v-btn text>👉🏼Shop Now</v-btn>
            </v-flex>
            <v-flex md6 class>
              <!-- <v-img class="entry-img" :src="require('../assets/images/coffee.jpg')"></v-img> -->
            </v-flex>
          </v-row>
        </v-container>
      </v-img>
    </div>
    <div class="section-coffee-container">
      <v-container>
        <v-row class="section-coffee-list">
          <v-flex md3 class="coffee-col coffee-col-first">
            <v-icon>mdi-feather</v-icon>
            <p>Quality Coffee Cultivated by Good</p>
          </v-flex>
          <v-flex md3 class="coffee-col">
            <v-icon>mdi-kodi</v-icon>
            <p>Flavour single origin froth in spoon iced</p>
          </v-flex>
          <v-flex md3 class="coffee-col">
            <v-icon>mdi-flower</v-icon>
            <p>Milk grounduts chicory beans single origin</p>
          </v-flex>
          <v-flex md3 class="coffee-col">
            <v-icon>mdi-image-filter-vintage</v-icon>
            <p>Coffee irish robusta spoon robust</p>
          </v-flex>
        </v-row>
        <v-row no-gutters class="section-quality-coffee">
          <v-flex md6 class="quality-coffee-col">
            <v-img
              class="entry-img"
              :src="require('../assets/images/coffee-plant.jpg')"
              aspect-ratio="1.7"
            ></v-img>
          </v-flex>
          <v-flex md6 class="quality-coffee-col">
            <p>PREMIUN COFFEE</p>
            <h4>
              Quaity Coffee
              <br />Cultivated by Good
            </h4>
            <p>
              Our love for speciality coffee is never ending. With over 365 days a year at origin working with the best growers on the planet,
              only the best beans make the grade
            </p>
            <v-btn text>👉🏼Shop Now</v-btn>
          </v-flex>
        </v-row>
      </v-container>
    </div>
    <div class="section-best-deal">
      <v-container>
        <v-row align="center" justify="center" no-gutters class="best-deal-row">
          <v-flex m12 class="best-deal-header">
            <p>BUY NOW</p>
            <h4>Our Best Deal</h4>
            <p>Coffee company with a straightforward mission: to make an office and on the go cup of coofee that we'd like to drink ourselves</p>
          </v-flex>
        </v-row>
        <v-row align="center" justify="center" class="section-coffee-pack">
          <v-flex md4 class="coffee-pack-col">
            <v-img class="pack-img" :src="require('../assets/images/coffee_pack.jpg')"></v-img>
            <p>PLATINIUM</p>
            <h5>Noansa Platinium Blend</h5>
            <v-btn text>👉🏼$30.00</v-btn>
          </v-flex>
          <v-flex md4 class="coffee-pack-col">
            <v-img class="pack-img" :src="require('../assets/images/coffee_pack.jpg')"></v-img>
            <p>PLATINIUM</p>
            <h5>Noansa Platinium Blend</h5>
            <v-btn text>👉🏼$30.00</v-btn>
          </v-flex>
          <v-flex md4 class="coffee-pack-col">
            <v-img class="pack-img" :src="require('../assets/images/coffee_pack.jpg')"></v-img>
            <p>PLATINIUM</p>
            <h5>Noansa Platinium Blend</h5>
            <v-btn text>👉🏼$30.00</v-btn>
          </v-flex>
        </v-row>
      </v-container>
    </div>
    <div class="section-bean">
      <v-container>
        <v-row no-gutters class="section-quality-coffee">
          <v-flex md6 class="quality-coffee-col">
            <p>PREMIUN COFFEE</p>
            <h4>
              Quaity Coffee
              <br />Cultivated by Good
            </h4>
            <p>
              Our love for speciality coffee is never ending. With over 365 days a year at origin working with the best growers on the planet,
              only the best beans make the grade
            </p>
            <v-btn text>👉🏼Shop Now</v-btn>
          </v-flex>
          <v-flex md6 class="quality-coffee-col">
            <v-img
              class="entry-img"
              :src="require('../assets/images/coffee-plant.jpg')"
              aspect-ratio="1.7"
            ></v-img>
          </v-flex>
        </v-row>
        <div class="noansa-hashtag text-center">
          <h4>#NOANSACOFFEE</h4>
          <p>Coffee perfection since 1927</p>
        </div>
      </v-container>
      <div class="image-gallery">
        <v-row>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup1.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup2.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup5.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup3.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup4.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup6.jpg')"></v-img>
          </v-flex>
        </v-row>
        <v-row>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup6.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup5.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup4.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup1.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup2.jpg')"></v-img>
          </v-flex>
          <v-flex md2>
            <v-img class="gallery-content" :src="require('../assets/images/cup3.jpg')"></v-img>
          </v-flex>
        </v-row>
      </div>
      <div class="contact text-center">
        <h4>Would you like to hear from us?</h4>
        <p>Submi your email address for our newslater</p>
        <v-flex md4 class="text-center email-input">
          <v-text-field class="text-center" placeholder="yourmail@mail.com" required></v-text-field>
        </v-flex>
      </div>
    </div>
    <v-footer>
      <v-container>
        <span>Al rights reserved &copy; 2019</span>
        <span>+436 701 32 43 92</span>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      fixed: false,
      drawer: false // Hide mobile side menu by default
    };
  }
};
</script>
<style>
.v-application--wrap {
  color: #120c0a !important;
}
.premium-container {
  background-color: #f2efe4;
  min-height: 700px;
}
.coffee-image {
  height: 700px;
}
.coffee-image .v-image__image {
  background-position: right center !important;
  background-size: 63% !important;
}
.nav-item button {
  color: #8d8a82 !important;
}
.v-toolbar__title {
  color: #120c0a !important;
}
.v-toolbar__content {
  padding-right: 0;
  padding-left: 0;
}
.entry-fold-col {
  max-width: 500px !important;
}
.entry-fold-col button,
.quality-coffee-col button,
.coffee-pack-col button {
  padding: 10px 15px;
  border-radius: 20px;
  background-color: #ffcf5b;
  margin: 20px 0;
  color: #120c0a !important;
  font-weight: 400;
}
.quality-coffee-col {
  max-width: 500px !important;
}
.entry-fold-col h4 {
  font-size: 40px;
}
.entry-fold {
  margin-top: 40px;
}
.section-coffee-container,
.section-bean {
  background-color: #fff !important;
}
.section-quality-coffee,
.section-coffee-list {
  margin: 50px 0;
  align-items: center;
}
.section-quality-coffee,
.entry-fold {
  justify-content: space-between;
  margin-top: 120px;
}
.coffee-col {
  padding: 30px 45px !important;
}
.coffee-col p {
  font-size: 28px;
  font-weight: 400;
}
.coffee-col-first {
  background-color: #fef0ca;
  border-radius: 0 70px 0 0;
  position: relative;
}
.mdi-feather::before {
  z-index: 9;
}
.coffee-col-first::after {
  position: absolute;
  display: block;
  background-color: #ffcf5b;
  content: "";
  height: 120px;
  width: 100%;
  border-bottom-left-radius: 50%;
  border-bottom-right-radius: 50%;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  background-repeat: no-repeat;
  background-position: center;
}
.coffee-col .v-icon {
  color: #120c0a;
  font-size: 30px;
  line-height: 4;
}
.quality-coffee-col .entry-img {
  border-radius: 100% 100% 0 100%;
  width: 450px;
  height: 400px;
  object-fit: cover;
}
.section-best-deal {
  background-color: #fffded;
}
.best-deal-row {
  text-align: center !important;
  max-width: 600px;
  margin-right: 25%;
  margin-left: auto;
  margin-top: 150px;
  margin-bottom: -150px;
}
.section-best-deal .container {
  margin-bottom: 50px;
}
.quality-coffee-col p,
.best-deal-row p {
  margin: 0;
}
.quality-coffee-col h4,
.best-deal-row h4 {
  font-size: 24px;
  font-weight: 500;
  margin-bottom: 20px;
}
.section-coffee-pack {
  text-align: center;
}
.coffee-pack-col p {
  margin-top: 20px;
}
.coffee-pack-col .pack-img .v-image__image {
  background-size: 200px;
  background-position: center bottom !important;

  /* width: 50%;
  margin-right: 25%;
  margin-bottom: auto; */
}
.noansa-hashtag {
  margin-top: 80px;
}
.noansa-hashtag h4 {
  font-weight: 700;
  font-size: 28px;
}
.gallery-content {
  height: 250px;
}
.contact {
  background-color: #2f3135;
  padding: 60px 0 40px;
  color: #fff;
}
.contact p {
  margin-bottom: 0;
}
.email-input {
  justify-content: center;
  align-items: center;
  display: flex;
  margin-left: 33.3%;
}
input::placeholder {
  text-align: center;
}
.v-footer .container {
  display: flex;
  justify-content: space-between;
}
@media only screen and (max-width: 768px) {
  .entry-fold-col p,
  span.v-btn_content.entry-fold-col button {
    font-size: 14px !important;
  }
  .email-input {
    margin-left: 0 !important;
  }
  .entry-fold-col h4 {
    font-size: 24px;
  }
  .best-deal-row {
    margin: 0 !important;
  }
}
</style>