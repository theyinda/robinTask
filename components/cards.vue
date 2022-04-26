<template>
  <div class="container">
    <div class="card">
      <h4>{{ name }}</h4>
      <p class="amount">{{ amount }}<span class="month">/mo</span></p>
      <div class="cards">
        <div class="cardInfo">
          <img src="../assets/images/tick.svg" /><span class="core"
            >Core Chat Features</span
          >
        </div>
        <div class="cardInfo">
          <img src="../assets/images/tick.svg" /><span class="core"
            >10,000 Monthly Active Users</span
          >
        </div>
        <div class="cardInfo">
          <img src="../assets/images/tick.svg" /><span class="core"
            >MAU Overage Rate</span
          >
        </div>
        <div class="cardInfo">
          <img src="../assets/images/tick.svg" /><span class="core"
            >100 Concurrent Included</span
          >
        </div>
        <div class="cardInfo">
          <img src="../assets/images/tick.svg" /><span class="core"
            >Limited Message Storage</span
          >
        </div>
      </div>

      <nuxt-link to="/">
        <span class="get-started">Get Started</span
        ><img src="../assets/images/blue.svg" />
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    name: String,
    amount: String,
  },
}
</script>

<style scoped>
.container {
  background: #f5f7fc;
  border: 1px solid #4568d1;
  box-sizing: border-box;
  border-radius: 25px;
   width: 310px;
}
.card {
  padding: 30px;
}
.container h4 {
  font-weight: 700;
  font-size: 18px;
  line-height: 19px;
  color: #ea8d51;
}
.container .amount {
  font-weight: 700;
  font-size: 35px;
  line-height: 45px;
  padding: 10px 0 20px 0;
}
.month {
  font-size: 35px;
  font-weight: normal;
}
.cards {
  border-bottom: 1px solid #bbc1d6;
  margin-bottom: 27px;
}
.cardInfo {
  display: flex;
  margin-bottom: 20px;
  /* align-items: center; */
}
.core {
  padding-left: 20px;
}
.get-started {
  font-weight: 700;
  font-size: 16px;
  line-height: 20px;
  color: #4568d1;
  padding-right: 15px;
}
</style>
