<template>
  <div class="home-container">
    <header data-role="Header" class="home-header">
      <span class="home-text">
        <span class="home-text01">Ro</span>
        <span class="home-text02">flare</span>
      </span>
      <div class="home-container1">
        <div class="home-container2">
          <div class="home-container3">
            <div data-role="BurgerMenu" class="home-burger-menu">
              <svg viewBox="0 0 1024 1024" class="home-icon">
                <path
                  d="M128 554.667h768c23.552 0 42.667-19.115 42.667-42.667s-19.115-42.667-42.667-42.667h-768c-23.552 0-42.667 19.115-42.667 42.667s19.115 42.667 42.667 42.667zM128 298.667h768c23.552 0 42.667-19.115 42.667-42.667s-19.115-42.667-42.667-42.667h-768c-23.552 0-42.667 19.115-42.667 42.667s19.115 42.667 42.667 42.667zM128 810.667h768c23.552 0 42.667-19.115 42.667-42.667s-19.115-42.667-42.667-42.667h-768c-23.552 0-42.667 19.115-42.667 42.667s19.115 42.667 42.667 42.667z"
                ></path>
              </svg>
            </div>
          </div>
        </div>
        <navigation-links1
          text="Home"
          text2="Documentation"
          text4="Npm"
          rootClassName="navigation-links1-root-class-name8"
        ></navigation-links1>
      </div>
      <div class="home-btn-group">
        <a
          href="https://npmjs.com/package/roflare"
          target="_blank"
          rel="noreferrer noopener"
          class="home-register button"
        >
          <span>
            <span>Install</span>
            <br />
          </span>
        </a>
      </div>
    </header>
    <div class="home-hero">
      <div class="home-container4">
        <h1 class="home-text06">
          <span class="home-text07">Ro</span>
          <span>flare</span>
        </h1>
        <span class="home-text09">
          Effortlessly access ROBLOX&apos;s web API using a lightweight NPM
          package, complete with type definitions for seamless integration.
        </span>
        <div class="home-btn-group1">
          <a
            href="https://npmjs.com/package/roflare"
            target="_blank"
            rel="noreferrer noopener"
            class="home-register1 button"
          >
            <span>
              <span>Install</span>
              <br />
            </span>
          </a>
          <a
            href="https://docs.roflare.ml"
            target="_blank"
            rel="noreferrer noopener"
            class="home-register2 button"
          >
            <span>
              <span>Read the Documentation</span>
              <br />
            </span>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavigationLinks1 from '../components/navigation-links1'

export default {
  name: 'Home',
  components: {
    NavigationLinks1,
  },
  metaInfo: {
    title: 'Roflare',
    meta: [
      {
        property: 'og:title',
        content: 'Roflare',
      },
    ],
  },
}
</script>

<style scoped>
.home-container {
  width: 100%;
  display: flex;
  overflow: auto;
  min-height: 100vh;
  align-items: center;
  flex-direction: column;
  background-color: #111111;
}
.home-header {
  width: 100%;
  display: flex;
  max-width: var(--dl-size-size-maxwidth);
  align-items: center;
  padding-top: var(--dl-space-space-twounits);
  padding-left: var(--dl-space-space-threeunits);
  padding-right: var(--dl-space-space-threeunits);
  padding-bottom: var(--dl-space-space-twounits);
  justify-content: space-between;
}
.home-text {
  color: rgb(255, 255, 255);
  font-size: 20px;
  font-weight: 600;
}
.home-text01 {
  color: #ff4a4a;
  font-style: normal;
}
.home-text02 {
  font-weight: 400;
}
.home-container1 {
  flex: 0 0 auto;
  width: auto;
  height: auto;
  display: flex;
  align-items: space-between;
  flex-direction: column;
}
.home-container2 {
  flex: 0 0 auto;
  width: auto;
  height: auto;
  display: flex;
  align-items: space-between;
  flex-direction: column;
}
.home-container3 {
  flex: 0 0 auto;
  width: auto;
  height: auto;
  display: flex;
  align-items: space-between;
  flex-direction: column;
}
.home-burger-menu {
  display: none;
}
.home-icon {
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}
.home-btn-group {
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.home-register {
  color: rgb(255, 255, 255);
  width: 100px;
  height: 35px;
  font-size: 13.5px;
  font-style: normal;
  transition: 0.3s;
  font-weight: 600;
  border-radius: 10px;
  text-decoration: none;
  background-color: rgb(255, 74, 74);
}
.home-register:hover {
  background-color: #d63030;
}
.home-hero {
  width: 100%;
  display: flex;
  padding: var(--dl-space-space-threeunits);
  max-width: var(--dl-size-size-maxwidth);
  min-height: 80vh;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.home-container4 {
  display: flex;
  margin-right: var(--dl-space-space-threeunits);
  padding-right: var(--dl-space-space-threeunits);
  flex-direction: column;
}
.home-text06 {
  color: rgb(255, 255, 255);
  font-size: 3rem;
  max-width: 450px;
}
.home-text07 {
  color: #ff4a4a;
}
.home-text09 {
  color: rgb(255, 255, 255);
  font-style: normal;
  margin-top: var(--dl-space-space-unit);
  font-weight: 200;
  margin-bottom: var(--dl-space-space-unit);
}
.home-btn-group1 {
  gap: 3;
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: row;
}
.home-register1 {
  color: rgb(255, 255, 255);
  width: 100px;
  height: 35px;
  font-size: 13.5px;
  font-style: normal;
  transition: 0.3s;
  font-weight: 600;
  border-radius: 10px;
  text-decoration: none;
  background-color: rgb(255, 74, 74);
}
.home-register1:hover {
  background-color: #d63030;
}
.home-register2 {
  top: 0px;
  left: 115px;
  color: rgb(255, 255, 255);
  width: 201px;
  height: 35px;
  z-index: 100;
  position: absolute;
  font-size: 13.5px;
  font-style: normal;
  transition: 0.3s;
  font-weight: 600;
  border-color: #ffffff;
  border-style: solid;
  border-width: 0.01px;
  border-radius: 10px;
  text-decoration: none;
  background-color: transparent;
}
.home-register2:hover {
  color: #ff4a4a;
  background-color: #ffffff;
}
@media(max-width: 991px) {
  .home-hero {
    flex-direction: column;
  }
  .home-container4 {
    align-items: center;
    margin-right: 0px;
    margin-bottom: var(--dl-space-space-twounits);
    padding-right: 0px;
  }
  .home-text06 {
    text-align: center;
  }
  .home-text09 {
    text-align: center;
    padding-left: var(--dl-space-space-threeunits);
    padding-right: var(--dl-space-space-threeunits);
  }
}
@media(max-width: 767px) {
  .home-header {
    padding-left: var(--dl-space-space-twounits);
    padding-right: var(--dl-space-space-twounits);
  }
  .home-burger-menu {
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .home-btn-group {
    display: none;
  }
  .home-hero {
    padding-left: var(--dl-space-space-twounits);
    padding-right: var(--dl-space-space-twounits);
  }
  .home-text09 {
    padding-left: var(--dl-space-space-unit);
    padding-right: var(--dl-space-space-unit);
  }
}
@media(max-width: 479px) {
  .home-header {
    padding: var(--dl-space-space-unit);
  }
  .home-hero {
    padding-top: var(--dl-space-space-twounits);
    padding-left: var(--dl-space-space-unit);
    padding-right: var(--dl-space-space-unit);
    padding-bottom: var(--dl-space-space-twounits);
  }
  .home-container4 {
    margin-bottom: var(--dl-space-space-unit);
  }
  .home-btn-group1 {
    flex-direction: column;
  }
}
</style>
