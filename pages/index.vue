<template>
  <div>
    <Header />
    <AboutUs />
    <OurGames />
    <OurPartners />
    <Footer />
  </div>
</template>
<script>
import Header from '../components/header.vue';
import OurGames from '@/components/ourGames.vue';
import OurPartners from '@/components/ourPartners.vue';
import Footer from '@/components/footer.vue';
import AboutUs from '@/components/aboutUs.vue'
export default {
  name: "IndexPage",
  components: {
    Header,
    AboutUs,
    OurGames,
    OurPartners,
    Footer
  },
}
</script>
``