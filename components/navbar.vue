<template>
  <div class="">
    <div class="topnav" id="myTopnav" ref="myTopnav">
      <nuxt-link to="#" class="side-nav_item">
        <img src="../assets/images/logo.svg" />
      </nuxt-link>
      <div class="doing">
        <nuxt-link to="/" class="side-nav_item">
          <p class="nav-link">Pricing</p>
        </nuxt-link>
        <nuxt-link to="#Docs" class="side-nav_item">
          <p class="nav-link">Docs</p>
        </nuxt-link>
        <nuxt-link to="#UseCases" class="side-nav_item">
          <p class="nav-link">Use Cases</p>
        </nuxt-link>
        <nuxt-link to="#SDKs" class="side-nav_item">
          <p class="nav-link">SDKs</p>
        </nuxt-link>
        <nuxt-link to="#" class="side-nav_item">
          <p class="nav-link">Enterprise</p>
        </nuxt-link>
        <nuxt-link to="#Demo" class="side-nav_item">
          <p class="nav-link">Try Demo</p>
        </nuxt-link>
      </div>

      <div class="details">
        <nuxt-link to="#login" class="side-nav_item">
          <p class="nav-link sign">Sign in</p>
        </nuxt-link>
        <nuxt-link to="#started" class="side-nav_item">
          <button>Get Started</button>
        </nuxt-link>
      </div>
      <a href="javascript:void(0);" class="icon" @click="myFunction()">
        <img src="../assets/images/icon.png" />
      </a>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    myFunction() {
      const x = this.$refs.myTopnav
      if (x.className === 'topnav') {
        x.className += ' responsive'
      } else {
        x.className = 'topnav'
      }
    },
  },
}
</script>

<style scoped>
.topnav {
  overflow: hidden;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #ffff;
  padding: 15px 70px;
  box-shadow: 0px 10px 20px rgba(0, 104, 255, 0.09);
  margin: 0px auto;
}

.topnav a {
  float: left;
  display: block;
  padding: 14px 16px;
  text-decoration: none;
  font-weight: 700;
  font-size: 14px;
  line-height: 16px;
  text-align: center;
  align-items: center;
  color: #000;
  opacity: 0.7;
}

/* active */
a.nuxt-link-exact-active {
  font-weight: 700;
  font-size: 14px;
  line-height: 16px;
  text-align: center;
  color: #000;
  opacity: 0.2;
}

.topnav .icon {
  display: none;
  background: #0c1f55;
}

.details {
  display: flex;
  justify-content: center;
  align-items: center;
}
.sign {
  font-size: 14px;
  line-height: 18px;
  text-align: center;
  color: #476bd2;
  padding-right: 25px;
}
.details button {
  font-weight: 700;
  font-size: 14px;
  line-height: 18px;
  text-align: center;
  color: #fff;
  width: 131px;
  height: 40px;
  background: #476bd2;
  border-radius: 30.5px;
}

@media screen and (max-width: 1200px) {
  .topnav a:not(:first-child),
  .details a,
  .doing a {
    display: none;
  }
  .topnav a.icon {
    float: right;
    display: block;
  }
  .topnav {
    display: block;
  }
}

@media screen and (max-width: 900px) {
  .topnav.responsive {
    position: relative;
  }
  .topnav.responsive .icon {
    position: absolute;
    right: 0;
    top: 0;
  }
  .topnav.responsive a {
    float: none;
    display: block;
    text-align: left;
  }
}
</style>
