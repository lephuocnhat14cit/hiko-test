<template>
  <section class="about-us" id="about-us">
    <div class="content container">
      <div class="row">
        <div class="side-left col-12 col-md-6">
          <h2 class="title">{{ $t("aboutUs.sideLeft.title") }}</h2>
          <p class="description">
            {{ $t("aboutUs.sideLeft.description") }}
          </p>

          <div class="count-number row">
            <div class="users col-6 col-md-12">
              <p class="value">600 <span class="unit">M</span>+</p>
              <p class="label-left">{{ $t("aboutUs.sideLeft.users") }}</p>
            </div>

            <div class="games col-6 col-md-12">
              <p class="value">135+</p>
              <p class="label-left">{{ $t("aboutUs.sideLeft.games") }}</p>
            </div>
          </div>
        </div>

        <div class="side-right col-12 col-md-6">
          <ul class="list-items">
            <li class="item">
              <div class="item-icon">
                <img
                  src="../assets/images/contents/aboutUs/date.svg"
                  alt="Date"
                />
              </div>

              <div class="item-content">
                <h3>{{ $t("aboutUs.sideRight.time.title") }}</h3>
                <p>{{ $t("aboutUs.sideRight.time.description") }}</p>
              </div>
            </li>

            <li class="item">
              <div class="item-icon">
                <img
                  src="../assets/images/contents/aboutUs/design.svg"
                  alt="Design"
                />
              </div>

              <div class="item-content">
                <h3>{{ $t("aboutUs.sideRight.design.title") }}</h3>
                <p>{{ $t("aboutUs.sideRight.design.description") }}</p>
              </div>
            </li>

            <li class="item">
              <div class="item-icon">
                <img
                  src="../assets/images/contents/aboutUs/team.svg"
                  alt="Team"
                />
              </div>

              <div class="item-content">
                <h3>{{ $t("aboutUs.sideRight.team.title") }}</h3>
                <p>{{ $t("aboutUs.sideRight.team.description") }}</p>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>
