<template>
  <div class="container">
    <div class="logo">
      <img src="../assets/images/logo.svg" />
    </div>
    <ul id="myTopnav" ref="myTopnav" class="topnav">
      <!-- <nuxt-link to="/" class="logo">
       <img src="../assets/images/logo.svg" />
      </nuxt-link> -->
      <nuxt-link to="/" class="side-nav_item">
        <p class="nav-link">Pricing</p>
      </nuxt-link>
      <nuxt-link to="#Docs" class="side-nav_item">
        <p class="nav-link">Docs</p>
      </nuxt-link>
      <nuxt-link to="#Use Cases" class="side-nav_item">
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
    </ul>
    <div class="details">
      <nuxt-link to="#login" class="side-nav_item">
        <p class="nav-link sign">Sign in</p>
      </nuxt-link>
      <nuxt-link to="#started" class="side-nav_item">
        <button>Get Started</button>
      </nuxt-link>
      <a href="javascript:void(0);" class="icon" @click="myFunction()">
        <i class="fa fa-bars"></i>
      </a>
    </div>
    <!-- <div class="topnav" id="myTopnav">
  <a href="#home" class="active">Home</a>
  <a href="#news">News</a>
  <a href="#contact">Contact</a>
  <a href="#about">About</a>
  <a href="javascript:void(0);" class="icon" onclick="myFunction()">
    <i class="fa fa-bars"></i>
  </a>
</div> -->
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
.container {
  background: pink;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #FFFFFF;
  padding: 15px 0;
box-shadow: 0px 10px 20px rgba(0, 104, 255, 0.09);

}
.logo {
  margin-left: 5%;
}
.details {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-right: 5%;
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
.nav-link {
  font-weight: 700;
  font-size: 14px;
  line-height: 16px;
  text-align: center;
  /* opacity: 0.6; */
}
.topnav {
  overflow: hidden;
}

.topnav a {
  float: left;
  display: block;
  font-weight: 700;
  font-size: 14px;
  line-height: 16px;
  text-align: center;
  color: #000000;
  padding: 20px 16px;
  text-decoration: none;
  font-size: 17px;
}
a.nuxt-link-exact-active {
  font-weight: 700;
  font-size: 14px;
  line-height: 16px;
  text-align: center;
  color: #000;
  opacity: 0.2;
}
/* .topnav a:hover {
  background-color: #ddd;
  color: black;
} */

/* .topnav a.active {
  background-color: #04aa6d;
  color: white;
} */

.topnav .icon {
  display: none;
}

@media screen and (max-width: 600px) {
  .topnav a:not(:first-child) {
    display: none;
  }
  .topnav a.icon {
    float: right;
    display: block;
  }
}

@media screen and (max-width: 600px) {
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
