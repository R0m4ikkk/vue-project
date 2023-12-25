<script setup>
const responce = [
  {
    img: {
      src: '/ivan.png',
      alt: 'ivan'
    },
    name: 'Иван'
  },
  {
    img: {
      src: '/leha.png',
      alt: 'alex'
    },
    name: 'Алексей'
  },
  {
    img: {
      src: '/timur.png',
      alt: 'timur'
    },
    name: 'Тимур'
  },
  {
    img: {
      src: '/ivanov.png',
      alt: 'ivanov i i'
    },
    name: 'ИП Иванов И.И.'
  },
  {
    img: {
      src: '/v.png',
      alt: 'vika'
    },
    name: 'Виктория'
  },
  {
    img: {
      src: '/michael.png',
      alt: 'michael'
    },
    name: 'Михаил'
  },
  {
    img: {
      src: '/star.png',
      alt: ''
    },
    name: 'Здесь можете быть Вы'
  }
]
</script>

<template>
<section class="tech">
      <div class="container">
        <h2>
          Довольные клиенты
        </h2>
        <div class="row">
          <div class="col-6 col-md-4 col-lg-3"
               v-for="(item, index) in responce"
               :key="index"
          >
            <div class="tech__card">
              <div class="tech__card-img-wrap">
                <img :src="item.img.src" :alt="item.img.alt">
              </div>
              <div class="tech__card-name">{{item.name}}</div>
            </div>
          </div>
        </div>
      </div>
    </section>
</template>

<style scoped>

</style>