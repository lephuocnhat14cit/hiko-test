<template>
  <section id="our-games" class="our-games">
    <h3>{{ $t("ourGames.title") }}</h3>

    <div class="d-flex justify-content-center">
      <p class="description">{{ $t("ourGames.description") }}</p>
    </div>

    <div class="product-list">
      <div class="row">
        <div class="col-left col-6 col-md-6">
          <div class="row">
            <div class="col-12 col-md-6">
              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/eSpace.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.eSpace") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>

              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/pirates.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.pirates") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>

              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/magicTree.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.magicTree") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>
            </div>

            <div class="odd-col col-12 col-md-6">
              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/kingland.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.kingland") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>

              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/witchParty.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.witchParty") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>

              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/aborigines.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.aborigines") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>
            </div>
          </div>
        </div>

        <div class="col-right col-6 col-md-6">
          <div class="row">
            <div class="even-col-mobile col-12 col-md-6">
              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/theLastGame.png')})`,
                  }"
                >
                  <p class="product-name">
                    {{ $t("ourGames.theLastGame") }}
                  </p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>

              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/rocky.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.rocky") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>

              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/cinderella.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.cinderella") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>
            </div>

            <div class="odd-col col-12 col-md-6">
              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/gDragon.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.gDragon") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>

              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/blueFire.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.blueFire") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>

              <a href="#">
                <div
                  class="product"
                  :style="{
                    backgroundImage: `url(${require('../assets/images/contents/ourGames/egyptGame.png')})`,
                  }"
                >
                  <p class="product-name">{{ $t("ourGames.egyptGame") }}</p>
                  <p class="product-description">
                    {{ $t("ourGames.descriptionGame") }}
                  </p>
                </div>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>