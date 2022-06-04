<template>
  <div>
    <Header />
    <AboutUs />
    <OurGames />
    <OurPartners />
    <Footer />
    <ArrowDown />
  </div>
</template>
<script>
import Header from '../components/header.vue';
import OurGames from '@/components/ourGames.vue';
import OurPartners from '@/components/ourPartners.vue';
import Footer from '@/components/footer.vue';
import AboutUs from '@/components/aboutUs.vue';
import ArrowDown from '@/components/arrowDown.vue';
export default {
  name: "HomePage",
  components: {
    Header,
    AboutUs,
    OurGames,
    OurPartners,
    Footer,
    ArrowDown
  },
}
</script>