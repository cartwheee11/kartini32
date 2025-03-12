<template>
  <main class="main">
    <nav style="position: fixed; width: 100%; top: 0; z-index: 200">
      <div class="inner-nav content container" style="padding: 15px 0; margin-bottom: 0">
        <h3 class="logo" style="font-family: bebas; gin: 0; position: absolute; right: 20px">8 (903) 819 39 09</h3>
        <h3 style="margin: 0; font-family: bebas;">картины</h3>
      </div>

      <!-- <hr style="padding: 0; margin: 0" /> -->
    </nav>

    <div class="header-container-wrapper">
      <section class="container content is-large header-container">
        <h1 class="" style="margin-top: 57px">
          Доступные <br />
          картины в <br> Брянске
        </h1>
        <p>Мы радуем вас живописью уже более 25 лет, <br>и не собираемся остонавливаться</p>
        <a style="margin-top: 60px !important" href=" tel:+79038193909"><button
            class="button is-primary is-large is-responsive">Позвонить</button></a>
      </section>
    </div>

    <!-- <hr style="padding: 0; margin: 0" /> -->
    <section class="map-section">
      <div class="container">
        <div class="content is-large">
          <div class="columns ">
            <div class="column is-three-fifths">
              <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2387.8130800058975!2d34.354695961653356!3d53.239126934286816!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x412d58f8018b4617%3A0x9d894b4f3f2b0a90!2z0YPQuy4g0JXQvNC70Y7RgtC40L3QsCwgNDIsINCR0YDRj9C90YHQuiwg0JHRgNGP0L3RgdC60LDRjyDQvtCx0LsuLCAyNDEwNTA!5e0!3m2!1sru!2sru!4v1589579621495!5m2!1sru!2sru"
                height="100%" frameborder="0" style="border: 0; width: 100%" allowfullscreen="" aria-hidden="false"
                tabindex="0">
              </iframe>
            </div>

            <div class="column is-one-quarters">
              <div class="content is-medium address-part">
                <h1>Наш адрес</h1>
                <p>
                  <code>тц «Брянский»:</code> г. Брянск, Советский район, центральный рынок,
                  остановка «Строительный техникум», ул. Емлютина. д. 42, 1 этаж
                </p>

                <div>
                  <WorkTimeTable />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section>
      <div class="content container">
        <h1 style="font-size: 80px">
          <span class=" has-text-black-bis">В наличии имеется более 1000 картин.</span>
          Консультант подберет картину специально под ваш интерьер и бюджет. Также вы можете
          заказать у нас любой сюжет
        </h1>
        <a href="tel:+79038193909"><button
            class="button is-primary is-fullwidth is-large is-responsive">Позвонить</button></a>
      </div>
    </section>

    <section class="svetlana-section">
      <div class="container">
        <div class="columns">
          <div class="column is-three-fifths">
            <img style="width: 100%; border-radius: 50px;" src="../assets/images/svetlana.jpg" alt=""
              class="is-fluid" />
          </div>
          <div class="column svetlana-desk">
            <div class="content is-large"
              style="background-color: #fff; padding: 50px; height: 100%; border-radius: 50px;">
              <h1>Головко Светлана — Художник</h1>
              <p style="color: black !important; font-size: 20px;">
                Объединила вокруг себя коллектив лучших художников Брянска, чтобы предложить вам
                огромный выбор картин
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section>
      <div class="container">
        <div class="swiper">
          <div class="swiper-wrapper">
            <!-- Slides -->
            <div class="swiper-slide">
              <img src="../assets/images/swiper-images/1.jpeg" alt="" />
            </div>
            <div class="swiper-slide">
              <img src="../assets/images/swiper-images/2.jpeg" alt="" />
            </div>
            <div class="swiper-slide">
              <img src="../assets/images/swiper-images/3.jpeg" alt="" />
            </div>
          </div>
          <!-- If we need pagination -->
          <div class="swiper-pagination"></div>

          <!-- If we need navigation buttons -->
          <div class="swiper-button-prev"></div>
          <div class="swiper-button-next"></div>

          <!-- If we need scrollbar -->
          <div class="swiper-scrollbar"></div>
        </div>
      </div>
    </section>

    <hr style="padding: 0; margin: 0" />
    <section class="feedback-section">
      <div class="container">
        <div class="content is-large has-text-centered">
          <h1>Наши клиенты</h1>
        </div>
        <div class="columns">
          <div class="column">
            <div v-for="rev in reviews" :key="rev.text" class="card">
              <div class="card-content">
                <div class="media" style="align-items: center">
                  <div class="media-left">
                    <figure class="image is-48x48">
                      <img style="border-radius: 100%" :src="rev.avatar" alt="" />
                    </figure>
                  </div>

                  <div class="media-content">
                    <div class="content">
                      <p class="title is-4">{{ rev.name }}</p>
                    </div>
                  </div>
                  <img src="../assets/images/stars.png" alt="" />
                </div>

                <hr />
                <div class="content is-large is-responsive">{{ rev.text }}</div>
              </div>
            </div>
          </div>
          <div class="column">
            <div v-for="rev in reviews2" :key="rev.text" class="card">
              <div class="card-content">
                <div class="media" style="align-items: center">
                  <div class="media-left">
                    <figure class="image is-48x48">
                      <img style="border-radius: 100%" :src="rev.avatar" alt="" />
                    </figure>
                  </div>

                  <div class="media-content">
                    <div class="content">
                      <p class="title is-4">{{ rev.name }}</p>
                    </div>
                  </div>

                  <img src="../assets/images/stars.png" alt="" />
                </div>

                <hr />
                <div class="content is-large is-responsive">{{ rev.text }}</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <hr style="padding: 0; margin: 0" />

    <footer>
      <div class="container is-large content has-text-centered">
        <h1 class="title" style="font-size: 80px">8(903)819-39-09</h1>
        <p class="is-large">Позвоните по этому <br>номеру и получите скидку 10%</p>
        <p><a href="tel:+79038193909"><button class="button is-primary is-large is-responsive">Позвонить</button></a>
        </p>
      </div>
    </footer>
  </main>
</template>

<script setup>
import { onMounted, ref } from 'vue'

import Swiper from 'swiper'
import { Navigation, Pagination } from 'swiper/modules'
import 'swiper/css'
import 'swiper/css/navigation'

import revs from '../assets/reviews.json'

import WorkTimeTable from '../components/WorkTimeTable.vue'

const reviews = ref([])
const reviews2 = ref([])

onMounted(() => {
  //working with swiper
  new Swiper('.swiper', {
    modules: [Navigation, Pagination],
    navigation: {
      nextEl: '.swiper-button-next',
      prevEl: '.swiper-button-prev',
    },
    loop: true,

    slidesPerView: 1.2,
    spaceBetween: 20,
    breakpoints: {
      1000: {
        slidesPerView: 1.5,
      },
    },
  })

  //loading reviews
  const allRevs = revs
  allRevs.forEach((rev, id) => {
    if (id < 3) {
      reviews.value.push(rev)
    } else {
      reviews2.value.push(rev)
    }
  })
})
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

.svetlana-section {
  background-color: var(--accent-color);
}

p,
td {
  color: black;
}

main {
  background-color: var(--back-color) !important;
}

main .header-images img {
  top: 0;
  position: absolute;
  z-index: -1;
}

.header-container-wrapper {
  background-image: url(../assets/images/header-back.png);
  background-position: center;
  /* background-position-y: center; */
  background-repeat: no-repeat;
  background-size: cover;

}

.swiper {
  /* overflow: visible */
}

.swiper-slide img {
  border-radius: 50px;
}

code {
  background-color: black;
  color: white;
}

.swiper-button-next,
.swiper-button-prev {
  width: 80px;
  height: 80px;
  border-radius: 100px;
  background-color: var(--accent-color)
}

.swiper-button-next::after,
.swiper-button-prev::after {
  color: var(--back-color-2);
  font-size: 25px;
  font-weight: 1000;
}

.card {
  box-shadow: none;
  border-radius: 50px;
}

hr {
  background-color: #6f6f6f34;
}

h1,
h3,
h2 {
  font-family: Montserrat;
  color: var(--accent-color) !important;
}

.header-images {
  overflow-y: hidden !important;
  overflow: hidden !important;

  z-index: 0;
}

section {
  padding: 100px 0;
}

.map-section {
  background-color: var(--accent-color);
  z-index: 2;
  position: relative;
}

.map-section h1,
.map-section p,
.map-section tr,
.map-section td,
.map-section th {
  color: white !important
}

iframe {
  border-radius: 50px;
}

.address-part {
  /* background-color: var(--back-color-2); */
  background-color: #fff;

  padding: 50px;
  border-radius: 50px;
  /* position: absolute; */
  /* right: 0; */
  /* transform-origin: right; */
  /* transform: scale(0.75) translateY(-50px); */
  /* box-shadow: 0px 23px 37px 0px rgba(34, 60, 80, 0.12); */
  /* width: 500px; */
}

.address-part h1,
.address-part p,
.address-part tr,
.address-part td,
.address-part th {
  color: var(--accent-color) !important;
}


table,
tr,
td,
th {
  border-color: rgba(119, 119, 119, 0.258) !important;
}

.header-container-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  justify-items: center;
  height: 100vh;
  overflow-y: hidden !important;
  overflow: hidden !important;
}



button {
  background-color: var(--accent-color) !important;
  color: white !important;
  font-family: "Montserrat";
  border-radius: 100px !important;
}

.header-container {
  flex-grow: 0 !important;
}



.header-container h1 {
  font-size: 90px;
  /* text-transform: uppercase; */
  /* font-family: bebas; */
  margin-bottom: 30px;
}

.feedback-section {
  background-color: var(--accent-color);
}

.feedback-section h1 {
  color: white !important;
}


/* nav {
  text-align: center;
} */

footer {
  padding: 200px 50px;
}

@media (max-width: 1215px) {
  .svetlana-section h1 {
    font-size: 40px;
  }

  section {
    padding: 30px 15px;
  }
}

@media (max-width: 1000px) {
  /* nav {
    text-align: left;
  } */

  .inner-nav {
    padding-left: 20px !important;
  }

  .swiper-button-next,
  .swiper-button-prev {
    display: none !important;
  }

  .swiper {
    /* overflow: visible */
  }

  .swiper img {
    border-radius: 20px;
  }

  iframe {
    border-radius: 20px;
  }

  .address-part {
    padding: 20px;
    border-radius: 20px;
  }

  .card {
    margin: 0;
  }

  .svetlana-section h1 {
    font-size: 30px;
  }

  .svetlana-desk .content {
    padding: 30px !important;
  }

}

@media (max-width: 769px) {
  h1 {
    font-size: 40px !important;
  }

  iframe {
    height: 600px;
  }

  .header-container-wrapper {
    height: 90vh;
  }

  .card {
    border-radius: 20px;
  }

  .svetlana-desk .content {
    padding: 20px !important;
  }

  .svetlana-desk .content {
    border-radius: 20px !important;
  }
}
</style>
