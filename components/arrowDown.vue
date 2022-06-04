<template>
  <div id="arrow-down" :class="[{'up': position[1] > 200 }, 'arrow-down']" @click="[position[1] < 10 ? handleButtomScroll() : handleTopScroll()]">
    <img src="../assets/images/common/arrowDown.svg" alt="" />
  </div>
</template>

<script>
import windowScrollPosition from '../store/windowScrollPosition';

export default {
  name: 'ArrowDown',
  data() {
    return {
      dataPos: 0,
    };
  },
  mixins: [windowScrollPosition('position')],
  methods: {
     handleTopScroll (){
      const footerElement = document.getElementById("footer");
      const footerOffsetTop = footerElement?.offsetTop;
      window.scrollTo({
        top:  0,
        behavior: "smooth",
      });
    },
    handleButtomScroll (){
      const footerElement = document.getElementById("footer");
      const footerOffsetTop = footerElement?.offsetTop;
      window.scrollTo({
        top:  footerOffsetTop || 0,
        behavior: "smooth",
      });
    }
  }
}
</script>
