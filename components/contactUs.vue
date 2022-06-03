<template>
  <section id="contact-us" class="contact-us border-top">
    <div class="contact-us-wrapper row">
      <div class="col-12 col-md-3 information">
        <a href="/" title="Logo">
          <img src="../assets/images/common/logo.svg" alt="Logo" class="logo" />
        </a>
        <div class="social">
          <a href="#" title="Twitter">
            <img
              src="../assets/images/contents/contactUs/twitter.svg"
              alt="Twitter"
            />
          </a>
          <a href="#" title="Facebook">
            <img
              src="../assets/images/contents/contactUs/facebook.svg"
              alt="Facebook"
            />
          </a>
          <a href="#" title="Linkedin">
            <img
              src="../assets/images/contents/contactUs/linkedin.svg"
              alt="Linkedin"
            />
          </a>
        </div>
      </div>

      <div class="col-12 col-md-5 address">
        <h3>{{ $t("contactUs.address") }}</h3>
        <ul class="items">
          <li class="item d-flex">
            <div>
              <img
                src="../assets/images/contents/contactUs/location.svg"
                alt="Location"
              />
            </div>
            <div class="item-content-address">
              <p class="address-english">
                {{ $t("contactUs.addressForeign") }}
              </p>
              <p>
                {{ $t("contactUs.addressLocal") }}
              </p>
            </div>
          </li>
          <li class="item d-flex">
            <div>
              <img
                src="../assets/images/contents/contactUs/phone.svg"
                alt="Phone"
              />
            </div>
            <div class="item-content-phone d-flex align-items-center">
              <p>{{ $t("contactUs.phone") }}</p>
            </div>
          </li>
        </ul>
      </div>

      <div class="col-12 col-md-4 subscribe">
        <h3>{{ $t("contactUs.subscribe") }}</h3>
        <p class="description">{{ $t("contactUs.subscribeDescription") }}</p>
        <div>
          <div class="email">
            <input type="text" :placeholder="$t('contactUs.placeholder')" />
            <svg
              width="25"
              height="24"
              viewBox="0 0 25 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill="white"
                d="M14.93 18.8201C14.74 18.8201 14.55 18.7501 14.4 18.6001C14.11 18.3101 14.11 17.8301 14.4 17.5401L19.94 12.0001L14.4 6.46012C14.11 6.17012 14.11 5.69012 14.4 5.40012C14.69 5.11012 15.17 5.11012 15.46 5.40012L21.53 11.4701C21.82 11.7601 21.82 12.2401 21.53 12.5301L15.46 18.6001C15.31 18.7501 15.12 18.8201 14.93 18.8201Z"
              />
              <path
                fill="white"
                d="M20.83 12.75H4C3.59 12.75 3.25 12.41 3.25 12C3.25 11.59 3.59 11.25 4 11.25H20.83C21.24 11.25 21.58 11.59 21.58 12C21.58 12.41 21.24 12.75 20.83 12.75Z"
              />
            </svg>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>
