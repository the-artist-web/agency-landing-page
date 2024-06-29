<template>
  <Header />
  <main>
    <article>
      <Hero />
      <ListImg />
      <CustomList />
      <BgListImg />
    </article>
  </main>
  <Footer />
</template>

<script>
import Header from '@/components/Header.vue'
import Hero from '@/components/Hero.vue'
import ListImg from '@/components/ListImg.vue'
import CustomList from '@/components/CustomList.vue'
import BgListImg from '@/components/BgListImg.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    ListImg,
    CustomList,
    BgListImg,
    Footer
  }
}
</script>

<style>
#app {
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: column;
}
</style>
