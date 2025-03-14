<template>
  <main class="main">
    <nav class="fixed w-full z-50">
      <div class="font-bebas mt-4 text-accent container flex items-center justify-between">
        <span class="text-2xl leading-none">картины<br>брянск</span>
        <a href="tel:+79038193909"><span class="text-2xl bg-accent p-4 px-10 pb-3 rounded-full text-white">8 903
            819-39-09</span></a>
      </div>
    </nav>

    <div class="w-full overflow-hidden">
      <div class="header-container-wrapper h-[90vh] md:h-[100vh]" data-aos="zoom-out" data-aos-offset="20">
        <section class="container header-container">
          <h1 data-aos="fade-up" class="text-4xl md:text-8xl lg:text-9xl md:text-7xl">
            Доступные <br />
            картины в <br> Брянске
          </h1>
          <p data-aos="fade-up" data-aos-delay="200" class="">Мы радуем вас живописью уже более 25 лет <br
              class="hidden md:block">и не
            собираемся остонавливаться
          </p>
          <p data-aos="fade-up" data-aos-delay="400"><a href=" tel:+79038193909"><button class="">Позвонить</button></a>
          </p>
        </section>
      </div>
    </div>


    <!-- <hr style="padding: 0; margin: 0" /> -->
    <section class="map-section bg-accent">
      <div class="container">

        <div class="md:grid-cols-[1.5fr_1fr] grid gap-5">
          <div class="" data-aos="fade-up">
            <iframe class="rounded-4xl min-h-[400px]"
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2387.8130800058975!2d34.354695961653356!3d53.239126934286816!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x412d58f8018b4617%3A0x9d894b4f3f2b0a90!2z0YPQuy4g0JXQvNC70Y7RgtC40L3QsCwgNDIsINCR0YDRj9C90YHQuiwg0JHRgNGP0L3RgdC60LDRjyDQvtCx0LsuLCAyNDEwNTA!5e0!3m2!1sru!2sru!4v1589579621495!5m2!1sru!2sru"
              height="100%" frameborder="0" style="border: 0; width: 100%" allowfullscreen="" aria-hidden="false"
              tabindex="0">
            </iframe>
          </div>

          <div class="bg-white p-7 md:p-10 rounded-4xl" data-aos="fade-up" data-aos-delay="200">
            <div class="">
              <h1>Наш адрес</h1>
              <p class="text-accent">
                <code class="bg-accent text-white rounded-full p-1 px-2 pb-0.5">тц «Брянский»:</code> г. Брянск,
                Советский
                район,
                центральный
                рынок,
                остановка «Строительный техникум», ул. Емлютина. д. 42, 1 этаж
              </p>

              <div>
                <br>
                <WorkTimeTable />
              </div>
            </div>
          </div>
        </div>

        <p data-aos="fade-up"><a
            href="https://www.google.com/maps?ll=53.239211,34.355227&z=17&t=m&hl=ru&gl=RU&mapclient=embed&q=%D1%83%D0%BB.+%D0%95%D0%BC%D0%BB%D1%8E%D1%82%D0%B8%D0%BD%D0%B0,+42+%D0%91%D1%80%D1%8F%D0%BD%D1%81%D0%BA+%D0%91%D1%80%D1%8F%D0%BD%D1%81%D0%BA%D0%B0%D1%8F+%D0%BE%D0%B1%D0%BB.+241050"><button
              class="border-4 font-bold w-full sm:text-2xl md:text-3xl p-4 bg-none border-solid">Показать на карте
              google</button></a></p>
      </div>
    </section>

    <section class="bg-back-2">
      <div class="container">
        <h2 class="md:text-8xl text-accent font-black" data-aos="fade-right">
          <span class="text-black">В наличии имеется более 1000 картин.</span>
          Консультант подберет картину специально под ваш интерьер и бюджет.
        </h2>
        <p data-aos="fade-up"><a href="tel:+79038193909"><button
              class=" sm:text-2xl md:text-3xl p-4 w-full">Позвонить</button></a></p>
      </div>
    </section>

    <section class="svetlana-section">
      <div class="container">
        <div class="grid md:grid-cols-[2fr_1fr] gap-4">
          <div class="column is-three-fifths">
            <img data-aos="fade-up" class="w-full rounded-4xl" src="../assets/images/svetlana.webp" alt="" />
          </div>
          <div class="column svetlana-desk">
            <div data-aos="fade-up" data-aos-delay="200" class="rounded-4xl pt-10 pb-10 md:p-10 md:py-10 h-full">
              <p class="bg-back-2 rounded-full text-accent p-4 py-1 text-base font-mont font-bold inline">Художник
              </p>
              <h1 class="md:text-6xl mt-4">

                Головко<br>
                Светлана
              </h1>
              <p class="text-accent">
                Объединила вокруг себя коллектив лучших художников Брянска, чтобы предложить вам
                огромный выбор картин
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>



    <section class="bg-accent">
      <div class="container">
        <h2 data-aos="fade-up" class=" mb-10 md:mb-20 font-[750] text-white md:text-8xl">Заглядывай к нам: <br><span
            class="text-back-3">у
            нас
            огромный
            выбор</span>
        </h2>
        <div class="swiper">
          <div class="swiper-wrapper">
            <!-- Slides -->
            <div class="swiper-slide">
              <img src="../assets/images/swiper-images/1.webp" alt="" />
            </div>
            <div class="swiper-slide">
              <img src="../assets/images/swiper-images/2.webp" alt="" />
            </div>
            <div class="swiper-slide">
              <img src="../assets/images/swiper-images/3.webp" alt="" />
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

    <section class="feedback-section bg-back-2">
      <div class="container">
        <h1 data-aos="fade-up" class="md:text-8xl lg:text-9xl text-center">Наши клиенты</h1>
        <div class="md:columns-2 gap-4 break-after-column mt-10 md:mt-15">
          <div data-aos="fade-up" class="card p-7 md:p-10 bg-white rounded-3xl break-inside-avoid mb-4"
            v-for="rev in reviews" :key="rev.text">
            <div class="flex items-center justify-between">

              <div class="flex items-center">
                <img class="mr-4 rounded-full size-10" :src="rev.avatar" alt="" />
                <p class="md:text-2xl font-bold mt-0">{{ rev.name }}</p>
              </div>

              <div class=""><img src="../assets/images/stars.webp" alt="" /></div>

            </div>
            <!-- <br class="displa hidden md:block"> -->
            <!-- <hr class="displa hidden md:block"> -->

            <p class="">{{ rev.text }}</p>

          </div>

        </div>
      </div>
    </section>

    <hr style="padding: 0; margin: 0" />

    <footer class="py-30">
      <div data-aos="fade-up" class="container is-large content has-text-centered text-center">
        <h2 class="text-6xl">8 903 819-
          39-09</h2>
        <p class="">Позвоните по этому <br>номеру и получите скидку 10%</p>
        <p>
          <a href="tel:+79038193909">
            <button class="">Позвонить</button>
          </a>
        </p>
      </div>
    </footer>
  </main>
</template>

<script setup>
import { onMounted, ref } from 'vue'
import Swiper from 'swiper'
import { Navigation, Pagination } from 'swiper/modules'


import AOS from 'aos'
import 'aos/dist/aos.css'

import 'swiper/css'
import 'swiper/css/navigation'

import revs from '../assets/reviews.json'

import WorkTimeTable from '../components/WorkTimeTable.vue'

const reviews = ref([])

onMounted(() => {
  AOS.init({
    duration: 1000
  })
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
  allRevs.forEach((rev) => {
    reviews.value.push(rev)
  })
})
</script>

<style>
@reference "../assets/main.css";

.header-container-wrapper {
  background-image: url(../assets/images/header-back.webp);
  background-position: center;
  /* background-position-y: center; */
  background-repeat: no-repeat;
  background-size: cover;
}

.swiper-slide img {
  border-radius: 50px;
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

section {
  @apply py-10 md:py-25
}

.header-container-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  justify-items: center;

  overflow-y: hidden !important;
  overflow: hidden !important;
}

.header-container {
  flex-grow: 0 !important;
}


@media (max-width: 1000px) {

  .swiper-button-next,
  .swiper-button-prev {
    display: none !important;
    opacity: 0;
  }

  .swiper img {
    border-radius: 20px;
  }
}
</style>
