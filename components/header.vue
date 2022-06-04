<template>
  <section class="section-header">
    <header>
      <nav class="navbar navbar-inverse">
        <a href="/" class="logo" title="">
          <img src="../assets/images/common/logo.svg" alt="" />
        </a>
        <div class="menu">
          <ul class="nav navbar-nav">
            <li>
              <a class="hoverable nav-item" @click="navigateMenu('about-us')">
                {{ $t("menu.aboutUs") }}
              </a>
            </li>
            <li>
              <a class="hoverable nav-item" @click="navigateMenu('our-games')">
                {{ $t("menu.games") }}
              </a>
            </li>
            <li>
              <a class="hoverable nav-item" @click="navigateMenu('our-partners')">
                {{ $t("menu.partners") }}
              </a>
            </li>
            <li>
              <a class="hoverable nav-item" @click="navigateMenu('contact-us')">
                {{ $t("menu.contactUs") }}
              </a>
            </li>
            <b-nav-item-dropdown :key="$i18n.locale">
              <template #text>
                <img :src="
                  require('../assets/images/header/' + $i18n.locale + '.svg')
                " alt="" class="haha" />
              </template>
              <b-dropdown-item v-for="locale in $i18n.locales" ref="langMenu" :key="locale"
                :to="switchLocalePath(locale)" :disabled="$i18n.locale === locale" class="lang-menu">
                <img :src="require('../assets/images/header/' + locale + '.svg')" alt="" />
                {{ $t(`header.lang.${locale}`) }}
              </b-dropdown-item>
            </b-nav-item-dropdown>
          </ul>
        </div>
        <div class="menu-btn" @click="handleMenuMobile">
          <img src="../assets/images/header/menu.svg" alt="" />
        </div>
      </nav>
    </header>
    <div class="banner-event">
      <div class="title">{{ $t("banner.title") }}</div>
      <div class="count-down-wrapper">
        <div class="count-down">
          <div class="days">
            <p class="time-value">30</p>
            <p class="time-label">{{ $t("banner.time.days") }}</p>
          </div>

          <div class="colon">:</div>
          <div class="hours">
            <p class="time-value">18</p>
            <p class="time-label">{{ $t("banner.time.hours") }}</p>
          </div>

          <div class="colon">:</div>
          <div class="minutes">
            <p class="time-value">20</p>
            <p class="time-label">{{ $t("banner.time.minutes") }}</p>
          </div>

          <div class="colon">:</div>
          <div class="second">
            <p class="time-value">11</p>
            <p class="time-label">{{ $t("banner.time.second") }}</p>
          </div>
        </div>
      </div>
      <div class="description">
        <p>{{ $t("banner.description.descriptionOne") }}</p>
        <p>{{ $t("banner.description.descriptionTwo") }}</p>
      </div>
      <div class="email-wrapper">
        <div class="email">
          <input type="text" :placeholder="$t('banner.placeholder')" />
          <svg width="25" height="24" viewBox="0 0 25 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path fill="black"
              d="M14.93 18.8201C14.74 18.8201 14.55 18.7501 14.4 18.6001C14.11 18.3101 14.11 17.8301 14.4 17.5401L19.94 12.0001L14.4 6.46012C14.11 6.17012 14.11 5.69012 14.4 5.40012C14.69 5.11012 15.17 5.11012 15.46 5.40012L21.53 11.4701C21.82 11.7601 21.82 12.2401 21.53 12.5301L15.46 18.6001C15.31 18.7501 15.12 18.8201 14.93 18.8201Z" />
            <path fill="black"
              d="M20.83 12.75H4C3.59 12.75 3.25 12.41 3.25 12C3.25 11.59 3.59 11.25 4 11.25H20.83C21.24 11.25 21.58 11.59 21.58 12C21.58 12.41 21.24 12.75 20.83 12.75Z" />
          </svg>
        </div>
      </div>
    </div>
    <div :class="[{'open': isOpen}, 'menu-mobile modal']">
      <div class="control">
        <div class="lang-mobile">
          <b-nav-item-dropdown :key="$i18n.locale">
            <template #text>
              <img width="26px" :src="
                require('../assets/images/header/' + $i18n.locale + '.svg')
              " alt="" />
            </template>

            <b-dropdown-item v-for="locale in $i18n.locales" ref="langMenu" :key="locale" :to="switchLocalePath(locale)"
              :disabled="$i18n.locale === locale">
              <img :src="require('../assets/images/header/' + locale + '.svg')" alt="" />
              {{ $t(`header.lang.${locale}`) }}
            </b-dropdown-item>
          </b-nav-item-dropdown>
        </div>
        <div class="close-btn" @click="handleMenuMobile">
          <img src="../assets/images/header/closeButton.svg" alt="" />
        </div>
      </div>
      <div class="nav-mobile">
        <div class="item">
          <a @click="navigateMenu('about-us')">{{ $t("menu.aboutUs") }}</a>
        </div>
        <div class="item">
          <a @click="navigateMenu('our-games')">{{ $t("menu.games") }}</a>
        </div>
        <div class="item">
          <a @click="navigateMenu('our-partners')">{{ $t("menu.partners") }}</a>
        </div>
        <div class="item">
          <a @click="navigateMenu('contact-us')">{{ $t("menu.contactUs") }}</a>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Header',
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    // handle menu mobiless
    handleMenuMobile() {
      this.isOpen = !this.isOpen;
      if (this.isOpen) {
        document.body.style.overflow = "hidden";
      } else {
        document.body.style.overflow = "auto";
      }
    },

    // handle scroll menu 
    navigateMenu(id) {
      this.isOpen = false;
      const element = document.getElementById(id);
      const offsetTop = element.offsetTop;
      window.scrollTo({
        top: offsetTop,
        behavior: "smooth",
      });
    },
  },
};
</script>
