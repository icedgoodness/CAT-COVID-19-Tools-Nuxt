<template>
  <nav class="navigation-links-nav" v-bind:class="rootClassName">
    <span class="navigation-links-text">{{ Home }}</span>
    <span class="navigation-links-text1 heading">{{ Model }}</span>
    <span class="navigation-links-text2 heading">{{ About }}</span>
    <span class="navigation-links-text3 heading">{{ legal }}</span>
    <span class="navigation-links-text4 heading">{{ kontak }}</span>
    <span class="navigation-links-text5 heading">{{ enid }}</span>
  </nav>
</template>

<script>
export default {
  name: 'NavigationLinks',
  props: {
    kontak: {
      type: String,
      default: 'Contact',
    },
    legal: {
      type: String,
      default: 'Legal',
    },
    Model: {
      type: String,
      default: 'Model',
    },
    Home: {
      type: String,
      default: 'Home',
    },
    enid: {
      type: String,
      default: 'EN/ID',
    },
    About: {
      type: String,
      default: 'About CAT Covid-19',
    },
    rootClassName: String,
  },
}
</script>

<style scoped>
.navigation-links-nav {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  flex-direction: row;
}
.navigation-links-text {
  font-size: 18px;
  font-family: Farro;
  font-weight: 700;
  line-height: 1.15;
  text-transform: none;
  text-decoration: none;
}
.navigation-links-text1 {
  margin-left: var(--dl-space-space-twounits);
}
.navigation-links-text2 {
  margin-left: var(--dl-space-space-twounits);
}
.navigation-links-text3 {
  margin-left: var(--dl-space-space-twounits);
}
.navigation-links-text4 {
  margin-left: var(--dl-space-space-twounits);
}
.navigation-links-text5 {
  margin-left: var(--dl-space-space-twounits);
}














@media(max-width: 1200px) {
  .navigation-links-text1 {
    color: var(--dl-color-gray-black);
  }
}
@media(max-width: 767px) {
  .navigation-links-nav {
    align-items: flex-start;
    flex-direction: column;
  }
  .navigation-links-text1 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text2 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text3 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text4 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text5 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
}
</style>
