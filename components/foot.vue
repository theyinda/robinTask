<template>
  <div class="container">
    <div class="foot">
      <div class="footer-top">
        <div class="left">
          <h3>Ready to have a chat?</h3>
          <p>
            We’d love to talk about your messaging strategy and help make your
            software more conversational.
          </p>
        </div>

        <div class="right">
          <div class="buttons">
            <button class="sales">
              Talk To Sales
              <span><img src="../assets/images/black.svg" /></span>
            </button>
            <button class="robin">
              Try Robin <span><img src="../assets/images/black.svg" /></span>
            </button>
          </div>
        </div>
      </div>

      <div class="footer-bottom">
        <div class="left"><img src="../assets/images/robin.svg" /></div>

        <div class="bottom-right">
          <div class="reference">
            <div class="resources">
              <p class="text">resources</p>
              <ul class="">
                <nuxt-link to="/" class="item">
                  <p class="links">Documention</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">Developer API</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">Product Demos</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">Help Center</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">System Status</p>
                </nuxt-link>
              </ul>
            </div>
            <div class="company">
              <p class="text">company</p>
              <ul class="">
                <nuxt-link to="/" class="item">
                  <p class="links">About</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">Security & Privacy</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">Blog</p>
                </nuxt-link>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="lastFooter-bottom">
        <div class="left "><p class="copyrightyear">© 2021 Robin Inc.</p></div>

        <div class="lastBottom-right">
          <div class="copyright">
            <ul class="">
              <nuxt-link to="/" class="item">
                <p class="robin-links">Terms of Service</p>
              </nuxt-link>
              <nuxt-link to="/" class="item">
                <p class="robin-links">Privacy Policy</p>
              </nuxt-link>
              <nuxt-link to="/" class="item">
                <p class="robin-links">Cookie Settings</p>
              </nuxt-link>
              <nuxt-link to="/" class="item">
                <p class="robin-links">Sub-Processors</p>
              </nuxt-link>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'foot',
}
</script>

<style scoped>
.container {
  /* background: #0c1f55; */
  background: red;
  width: 100%;
  max-width: 1440px;
  margin: 0px auto;
  /* margin-right: 0px !important; */
}
.foot {
  width: 90%;
  margin: 0 auto;
}
.footer-top {
  padding-top: 70px;
  display: flex;
  justify-content: space-between;
}
.left h3 {
  font-weight: 700;
  font-size: 43px;
  line-height: 51px;
  color: #fff;
}
.left p {
  font-weight: 400;
  font-size: 20px;
  line-height: 35px;
  color: #ffffff;
  width: 526px;
  opacity: 0.7;
  padding-top: 23px;
}
.buttons {
  display: flex;
}
.buttons button {
  border-radius: 30.5px;
  font-weight: 700;
  font-size: 16px;
  line-height: 20px;
  text-align: center;
  color: #fff;
  width: 207px;
  height: 50px;
}
.sales {
  margin-right: 15px;
  background: #4568d1;
}
.robin {
  background: transparent;
  border: 1px solid #4568d1;
}
span img {
  margin-left: 20px;
}
.footer-bottom {
  /* width: 100%; */
  /* opacity: 0.1; */
  padding-top: 40px;
  border-top: 1px solid #ffffff;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
  display: flex;
  justify-content: space-between;
  margin: 30px auto;
}
.lastFooter-bottom {
  width: 100%;
  padding-top: 20px;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.bottom-right {
  width: 25%;
}
.reference {
  display: flex;
  justify-content: space-between;
}
.resources .text,
.company .text {
  font-weight: 700;
  font-size: 13px;
  line-height: 17px;
  color: #fff;
  opacity: 0.4;
  text-transform: uppercase;
}
.links {
  font-weight: 600;
  font-size: 12px;
  line-height: 14px;
  color: #fff;
  padding-top: 20px;
}
.lastBottom-right {
  width: 60%;
}
.copyright ul {
  width: 100%;
  display: flex;
  justify-content: space-around;
}
.robin-links {
  font-weight: 400;
  font-size: 13px;
  line-height: 17px;
  color: #fff;
  opacity: 0.5;
  padding: 20px 0;
}
.copyrightyear {
  font-weight: 400;
  font-size: 14px !important;
  line-height: 18px;
  color: #fff;
  opacity: 0.3;
}
@media screen and (max-width: 1200px) {
  .footer-top {
    display: block;
  }
  .buttons {
    margin-top: 40px;
  }
  .footer-bottom {
    display: block;
  }
  .bottom-right {
    width: 100%;
  }
  .reference {
    width: 100%;
    margin-top: 30px;
    justify-content: space-between;
  }
  .lastBottom-right {
    width: 100%;
  }
  .lastFooter-bottom {
    width: 100%;
    display: block;
    justify-content: center;
    /* align-items: center; */
    margin: 0 auto;
  }
  .copyright ul {
    width: 100%;
  }
  .robin-links {
    font-weight: 400;
    font-size: 13px;
    line-height: 17px;
    color: #fff;
    opacity: 0.5;
    padding: 20px 0;
  }
}
@media screen and (max-width: 600px) {
  .buttons {
    display: block;
    margin-top: 40px;
  }
  .buttons button {
    margin-bottom: 30px;
  }
  .left p {
    font-weight: 400;
    font-size: 20px;
    line-height: 35px;
    color: #ffffff;
    opacity: 0.7;
    width: 300px;
  }
  .copyright ul {
    display: block;
  }
}
</style>
