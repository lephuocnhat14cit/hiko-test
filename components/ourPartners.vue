<template>
  <section id="our-partners" class="our-partners">
    <h3>{{ $t("ourPartners.title") }}</h3>
    <div>
      <Flickity
        id="our-partner-carousel"
        ref="flickity"
        :options="flickityOptions"
      >
        <div class="slide">
          <img src="../assets/images/contents/ourPartners/eAGame.svg" alt="" />
        </div>
        <div class="slide">
          <img src="../assets/images/contents/ourPartners/game.svg" alt="" />
        </div>
        <div class="slide">
          <img
            src="../assets/images/contents/ourPartners/firstPowerUp.svg"
            alt=""
          />
        </div>
        <div class="slide">
          <img
            src="../assets/images/contents/ourPartners/waltDisney.png"
            alt=""
          />
        </div>
        <div class="slide">
          <img
            src="../assets/images/contents/ourPartners/bookProGameShow.svg"
            alt=""
          />
        </div>
        <div class="slide">
          <img src="../assets/images/contents/ourPartners/sega.svg" alt="" />
        </div>
        <div class="slide">
          <img src="../assets/images/contents/ourPartners/2k.svg" alt="" />
        </div>
      </Flickity>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      flickityOptions: {
        initialIndex: 0,
        prevNextButtons: true,
        pageDots: false,
        wrapAround: true,
        cellAlign: "left",
      },
    };
  },
};
</script>