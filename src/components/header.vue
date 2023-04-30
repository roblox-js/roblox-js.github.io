<template>
  <div data-role="Header" class="header-header">
    <nav class="header-nav">
      <div class="header-container">
        <router-link to="/" class="header-navlink Large">ROBLOX.JS</router-link>
        <div class="header-menu">
          <router-link to="/" class="header-navlink1 Large">Home</router-link>
          <a
            href="https://github.com/roblox-js/core"
            target="_blank"
            rel="noreferrer noopener"
            class="header-link Large"
          >
            Github
          </a>
          <a
            href="https://roblox-js.github.io/docs"
            target="_blank"
            rel="noreferrer noopener"
            class="header-link1 Large"
          >
            Docs
          </a>
        </div>
        <div class="header-container1">
          <div class="header-container2">
            <a
              href="https://npmjs.com/package/roblox.js"
              target="_blank"
              rel="noreferrer noopener"
              class="header-link2"
            >
              <primary-pink-button
                button="INSTALL"
                class="header-component"
              ></primary-pink-button>
            </a>
          </div>
          <div data-role="BurgerMenu" class="header-burger-menu">
            <svg viewBox="0 0 1024 1024" class="header-icon">
              <path
                d="M128 256h768v86h-768v-86zM128 554v-84h768v84h-768zM128 768v-86h768v86h-768z"
              ></path>
            </svg>
          </div>
        </div>
      </div>
    </nav>
    <div data-role="MobileMenu" class="header-mobile-menu">
      <div class="header-top">
        <router-link to="/" class="header-navlink2 Large">
          Soft UI Design System
        </router-link>
        <div data-role="CloseMobileMenu" class="header-close-menu">
          <svg viewBox="0 0 1024 1024" class="header-icon2">
            <path
              d="M810 274l-238 238 238 238-60 60-238-238-238 238-60-60 238-238-238-238 60-60 238 238 238-238z"
            ></path>
          </svg>
        </div>
      </div>
      <div class="header-mid">
        <div class="header-menu1">
          <router-link to="/" class="header-navlink3 Large">Home</router-link>
          <router-link to="/profile" class="header-navlink4 Large">
            Profile
          </router-link>
          <router-link to="/coming-soon" class="header-navlink5 Large">
            Coming Soon
          </router-link>
        </div>
      </div>
      <div class="header-bot">
        <primary-pink-button button="buy now"></primary-pink-button>
      </div>
    </div>
  </div>
</template>

<script>
import PrimaryPinkButton from './primary-pink-button'

export default {
  name: 'Header',
  props: {},
  components: {
    PrimaryPinkButton,
  },
}
</script>

<style scoped>
.header-header {
  top: 0px;
  left: auto;
  right: auto;
  width: 100%;
  bottom: auto;
  display: flex;
  z-index: 3;
  position: fixed;
  max-width: 1320px;
  padding-left: var(--dl-space-space-unitandahalfunit);
  padding-right: var(--dl-space-space-unitandahalfunit);
  justify-content: center;
}
.header-nav {
  flex: 0 0 auto;
  color: var(--dl-color-secondary-600);
  width: 100%;
  height: 60px;
  display: flex;
  flex-wrap: wrap;
  box-shadow: 0 .25rem .375rem -.0625rem hsla(0,0%,8%,.12),0 .125rem .25rem -.0625rem hsla(0,0%,8%,.07)!important;
  margin-top: var(--dl-space-space-unit);
  align-items: center;
  padding-top: var(--dl-space-space-halfunit);
  padding-left: var(--dl-space-space-unitandahalfunit);
  border-radius: var(--dl-radius-radius-radius40);
  padding-right: var(--dl-space-space-unitandahalfunit);
  flex-direction: row;
  padding-bottom: var(--dl-space-space-halfunit);
  backdrop-filter: saturate(200%) blur(30px);
  justify-content: space-between;
  background-color: hsla(0,0%,100%,.8)!important;
}
.header-container {
  color: var(--dl-color-gray-black);
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.header-navlink {
  color: var(--dl-color-secondary-700);
  font-weight: 600;
  margin-left: var(--dl-space-space-unit);
  margin-right: var(--dl-space-space-unit);
  text-decoration: none;
}
.header-menu {
  flex: 0 0 auto;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
}
.header-navlink1 {
  margin-top: var(--dl-space-space-halfunit);
  transition: 0.3s;
  margin-left: var(--dl-space-space-unit);
  margin-right: var(--dl-space-space-unit);
  margin-bottom: var(--dl-space-space-halfunit);
  text-decoration: none;
}
.header-navlink1:hover {
  color: var(--dl-color-gray-500);
}
.header-link {
  margin-top: var(--dl-space-space-halfunit);
  transition: 0.3s;
  margin-left: var(--dl-space-space-unit);
  margin-right: var(--dl-space-space-unit);
  margin-bottom: var(--dl-space-space-halfunit);
  text-decoration: none;
}
.header-link:hover {
  color: var(--dl-color-gray-500);
}
.header-link1 {
  margin-top: var(--dl-space-space-halfunit);
  transition: 0.3s;
  margin-left: var(--dl-space-space-unit);
  margin-right: var(--dl-space-space-unit);
  margin-bottom: var(--dl-space-space-halfunit);
  text-decoration: none;
}
.header-link1:hover {
  color: var(--dl-color-gray-500);
}
.header-container1 {
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.header-container2 {
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.header-link2 {
  display: contents;
}
.header-component {
  text-decoration: none;
}
.header-burger-menu {
  display: none;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.header-icon {
  width: 24px;
  height: 24px;
  margin-left: var(--dl-space-space-unit);
}
.header-mobile-menu {
  top: 0px;
  flex: 0 0 auto;
  left: 0px;
  width: 100%;
  height: 100vh;
  display: none;
  padding: var(--dl-space-space-unitandahalfunit);
  z-index: 100;
  position: absolute;
  align-items: flex-start;
  flex-direction: column;
  background-color: var(--dl-color-gray-white);
}
.header-top {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  padding: var(--dl-space-space-unit);
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.header-navlink2 {
  color: var(--dl-color-secondary-700);
  font-weight: 600;
  text-decoration: none;
}
.header-close-menu {
  flex: 0 0 auto;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.header-icon2 {
  width: 24px;
  height: 24px;
}
.header-mid {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  padding-left: var(--dl-space-space-unit);
  padding-right: var(--dl-space-space-unit);
  flex-direction: column;
}
.header-menu1 {
  flex: 0 0 auto;
  display: flex;
  align-items: flex-start;
  margin-bottom: var(--dl-space-space-unit);
  flex-direction: column;
}
.header-navlink3 {
  transition: 0.3s;
  margin-bottom: var(--dl-space-space-halfunit);
  text-decoration: none;
}
.header-navlink3:hover {
  color: var(--dl-color-gray-500);
}
.header-navlink4 {
  transition: 0.3s;
  margin-bottom: var(--dl-space-space-halfunit);
  text-decoration: none;
}
.header-navlink4:hover {
  color: var(--dl-color-gray-500);
}
.header-navlink5 {
  transition: 0.3s;
  text-decoration: none;
}
.header-navlink5:hover {
  color: var(--dl-color-gray-500);
}
.header-bot {
  flex: 0 0 auto;
  display: flex;
  margin-top: auto;
  flex-direction: column;
}
@media(max-width: 991px) {
  .header-nav {
    max-width: 960px;
  }
  .header-menu {
    display: none;
  }
}
@media(max-width: 767px) {
  .header-burger-menu {
    display: flex;
  }
}
@media(max-width: 479px) {
  .header-container2 {
    display: none;
  }
}
</style>
