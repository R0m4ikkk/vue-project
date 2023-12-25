<script setup>
const cars = [
  {
    img: {
      src: '/civic.png',
      alt: 'Honda Civic'
    },
    link: {
      href: '#',
      title: 'Хонда Сивик'
    },
    description: 'Комфортный седан среднего класса'
  },
  {
    img: {
      src: '/bmw3.png',
      alt: 'BMW3'
    },
    link: {
      href: '#',
      title: 'БМВ 3 серии'
    },
    description: 'Резвая спортивная трехлитровая'
  },
  {
    img: {
      src: '/mercedes_s.png',
      alt: 'mercedes_s_class'
    },
    link: {
      href: '#',
      title: 'Мерседес С класс'
    },
    description: 'Лакшери купе для тех, кто хочет больше...'
  },
  {
    img: {
      src: '/multivan.png',
      alt: 'vw multivan'
    },
    link: {
      href: '#',
      title: 'Фольксваген мультивэн'
    },
    description: 'Отличный семейный минивен под различные цели'
  },
  {
    img: {
      src: '/macan.png',
      alt: 'Macan'
    },
    link: {
      href: '#',
      title: 'Порше макан'
    },
    description: 'Спортивный кроссовер премиум класса'
  },
  {
    img: {
      src: '/lada_vesta.png',
      alt: 'Lada Vesta'
    },
    link: {
      href: '#',
      title: 'Лада Веста спорт'
    },
    description: 'Городская зажигалка, которая подойдет и для трека'
  },
  {
    img: {
      src: '/gazelle.png',
      alt: 'gazelle'
    },
    link: {
      href: '#',
      title: 'Газель NEXT'
    },
    description: 'Коммерческие новые газели'
  }
]
</script>

<template>
  <section class="projects">
    <div class="container">
      <h2>
        Наш автопарк
      </h2>
      <div class="row">
        <div class="col-sm-6 col-lg-4"
             v-for="(item, index) in cars"
             :key="index"
        >
          <div class="projects__card">
            <img :src="item.img.src"
                 :alt="item.img.alt"
            >
            <a :href="item.link.href">{{ item.link.title }}</a>
            <p>{{ item.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>

</style>