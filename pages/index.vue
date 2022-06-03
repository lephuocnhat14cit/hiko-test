<template>
  <div>
    <Header />
    <AboutUs />
    <AnimationArea />
    <OurGames />
    <OurPartners />
    <ContactUs />
    <Footer />
  </div>
</template>

<script>
import Tutorial from '../components/Tutorial.vue';
import Header from '../components/header.vue';
import AnimationArea from '@/components/animationArea.vue';
import OurGames from '@/components/ourGames.vue';
import OurPartners from '@/components/ourPartners.vue';
import ContactUs from '@/components/contactUs.vue';
import Footer from '@/components/footer.vue';
import AboutUs from '@/components/aboutUs.vue'
export default {
  name: "IndexPage",
  components: {
    Tutorial,
    Header,
    AnimationArea,
    OurGames,
    OurPartners,
    ContactUs,
    Footer,
    AboutUs
  },
  methods: {
    handleClick () {
      console.log('hahahah');
    }
  }  
}
</script>
