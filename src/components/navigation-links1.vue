<template>
  <nav class="navigation-links1-nav" v-bind:class="rootClassName">
    <router-link to="/" class="navigation-links1-navlink">{{ text }}</router-link>
    <a
      href="https://github.com/roblox-js/core"
      target="_blank"
      rel="noreferrer noopener"
      class="navigation-links1-link"
    >
      {{ text2 }}
    </a>
    <a
      href="https://npmjs.com/package/roflare"
      target="_blank"
      rel="noreferrer noopener"
      class="navigation-links1-link1"
    >
      {{ text4 }}
    </a>
  </nav>
</template>

<script>
export default {
  name: 'NavigationLinks1',
  props: {
    text4: {
      type: String,
      default: 'Blog',
    },
    rootClassName: String,
    text2: {
      type: String,
      default: 'Pricing',
    },
    text1: {
      type: String,
      default: 'Features',
    },
    text: {
      type: String,
      default: 'About',
    },
    text3: {
      type: String,
      default: 'Team',
    },
  },
}
</script>

<style scoped>
.navigation-links1-nav {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  flex-direction: row;
}
.navigation-links1-navlink {
  color: #FF4A4A;
  text-decoration: none;
}
.navigation-links1-link {
  color: #ffffff;
  margin-left: var(--dl-space-space-twounits);
  text-decoration: none;
}
.navigation-links1-link1 {
  color: #ffffff;
  margin-left: var(--dl-space-space-twounits);
  text-decoration: none;
}









@media(max-width: 767px) {
  .navigation-links1-nav {
    align-items: flex-start;
    flex-direction: column;
  }
  .navigation-links1-navlink {
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links1-link {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links1-link1 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
}
</style>
