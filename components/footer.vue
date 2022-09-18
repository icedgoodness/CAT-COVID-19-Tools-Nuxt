<template>
  <footer class="footer-footer" v-bind:class="rootClassName">
    <div class="footer-separator">
      <img :alt="image_alt" :src="image_src" class="footer-image" />
      <img :alt="image_alt1" :src="image_src1" class="footer-image1" />
      <img :alt="image_alt2" :src="image_src2" class="footer-image2" />
      <img :alt="image_alt3" :src="image_src3" class="footer-image3" />
      <img :alt="image_alt4" :src="image_src4" class="footer-image4" />
      <img :alt="image_alt5" :src="image_src5" class="footer-image5" />
      <img :alt="image_alt6" :src="image_src6" class="footer-image6" />
    </div>
    <div class="footer-container">
      <span class="footer-text">{{ text }}</span>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    rootClassName: String,
    image_alt: {
      type: String,
      default: 'image',
    },
    image_src6: {
      type: String,
      default: '/playground_assets/logo%20rspiss.svg',
    },
    image_src3: {
      type: String,
      default: '/playground_assets/logo%20imeri.svg',
    },
    image_src4: {
      type: String,
      default: '/playground_assets/logo%20rsui.svg',
    },
    image_alt6: {
      type: String,
      default: 'image',
    },
    image_alt2: {
      type: String,
      default: 'image',
    },
    image_alt4: {
      type: String,
      default: 'image',
    },
    image_alt5: {
      type: String,
      default: 'image',
    },
    image_alt3: {
      type: String,
      default: 'image',
    },
    text: {
      type: String,
      default: '© 2022 All Rights Reserved.',
    },
    image_src: {
      type: String,
      default: '/playground_assets/logo%20fkui.svg',
    },
    image_alt1: {
      type: String,
      default: 'image',
    },
    image_src1: {
      type: String,
      default:
        '/playground_assets/departemen%20pulmonologi%20dan%20kedokteran%20respirasi.svg',
    },
    image_src5: {
      type: String,
      default: '/playground_assets/logo%20rs%20persahabatan.svg',
    },
    image_src2: {
      type: String,
      default: '/playground_assets/logo%20medtech%20hd%20%201.svg',
    },
  },
}
</script>

<style scoped>
.footer-footer {
  width: 100%;
  display: flex;
  z-index: 3;
  position: relative;
  max-width: auto;
  margin-top: var(--dl-space-space-unit);
  align-items: stretch;
  padding-top: var(--dl-space-space-twounits);
  padding-left: 0px;
  padding-right: 0px;
  flex-direction: row;
  padding-bottom: var(--dl-space-space-twounits);
  justify-content: space-between;
  background-color: var(--dl-color-primary-putihgading);
}
.footer-separator {
  flex: 0 0 auto;
  width: 100%;
  height: auto;
  display: flex;
  position: relative;
  margin-top: var(--dl-space-space-twounits);
  object-fit: scale-down;
  align-items: flex-start;
  margin-left: right;
  margin-right: right;
  margin-bottom: var(--dl-space-space-twounits);
  flex-direction: row;
  background-size: cover;
  justify-content: center;
}
.footer-image {
  width: auto;
  margin: var(--dl-space-space-halfunit);
  align-self: center;
  object-fit: contain;
}
.footer-image1 {
  width: max-content;
  margin: var(--dl-space-space-halfunit);
  align-self: center;
  object-fit: contain;
}
.footer-image2 {
  width: max-content;
  margin: var(--dl-space-space-halfunit);
  align-self: center;
  object-fit: contain;
}
.footer-image3 {
  width: max-content;
  margin: var(--dl-space-space-halfunit);
  align-self: center;
  object-fit: contain;
}
.footer-image4 {
  width: max-content;
  margin: var(--dl-space-space-halfunit);
  align-self: center;
  object-fit: contain;
}
.footer-image5 {
  width: 140px;
  margin: var(--dl-space-space-halfunit);
  align-self: center;
  object-fit: contain;
}
.footer-image6 {
  width: max-content;
  margin: var(--dl-space-space-halfunit);
  align-self: center;
  object-fit: contain;
}
.footer-container {
  flex: 0 0 auto;
  left: 0px;
  right: 0px;
  width: 100%;
  bottom: 0px;
  display: flex;
  position: absolute;
  align-items: center;
  padding-top: var(--dl-space-space-halfunit);
  flex-direction: row;
  padding-bottom: var(--dl-space-space-halfunit);
  justify-content: center;
  background-color: var(--dl-color-primary-hijautua);
}
.footer-text {
  color: var(--dl-color-gray-white);
}

@media(max-width: 1200px) {
  .footer-footer {
    height: auto;
    padding-top: 0px;
    flex-direction: column;
    padding-bottom: 0px;
  }
  .footer-separator {
    flex-wrap: wrap;
    padding-left: var(--dl-space-space-halfunit);
    padding-right: var(--dl-space-space-halfunit);
  }
  .footer-image {
    width: auto;
    height: 85px;
  }
  .footer-image1 {
    width: auto;
  }
  .footer-image2 {
    width: auto;
  }
  .footer-image3 {
    width: 70px;
    height: 78px;
  }
  .footer-image4 {
    width: 70px;
    height: 78px;
  }
  .footer-image6 {
    width: 70px;
    height: auto;
  }
  .footer-container {
    position: static;
    align-self: flex-end;
    padding-top: var(--dl-space-space-halfunit);
    padding-bottom: var(--dl-space-space-halfunit);
  }
  .footer-text {
    font-size: 12px;
  }
}
@media(max-width: 991px) {
  .footer-footer {
    margin-top: var(--dl-space-space-twounits);
  }
}
@media(max-width: 767px) {
  .footer-footer {
    padding: 0px;
  }
  .footer-separator {
    margin-top: var(--dl-space-space-oneandhalfunits);
    margin-left: 0px;
    margin-right: 0px;
    margin-bottom: var(--dl-space-space-oneandhalfunits);
  }
  .footer-container {
    align-items: center;
    flex-direction: column;
    justify-content: center;
  }
  .footer-text {
    margin: var(--dl-space-space-halfunit);
  }
}
@media(max-width: 650px) {
  .footer-footer {
    padding: 0px;
  }
  .footer-separator {
    margin-top: var(--dl-space-space-oneandhalfunits);
    margin-bottom: var(--dl-space-space-oneandhalfunits);
  }
  .footer-container {
    align-items: center;
    flex-direction: column;
    justify-content: space-between;
  }
  .footer-text {
    text-align: center;
    margin-bottom: var(--dl-space-space-oneandhalfunits);
  }
}
</style>
