<template>
  <div class="all">
    <navbar />
    <div class="over-all">
      <div class="hero-container">
        <h3>Simple & Transparent Pricing. No surprises.</h3>
        <p>The only tool you will need to power conversations.</p>
        <button>
          Start Free Trial <span><img src="../assets/images/black.svg" /></span>
        </button>
      </div>
      <div class="card-container">
        <cards :name="cardNameOne" :amount="cardAmountOne" />
        <cards :name="cardNameTwo" :amount="cardAmountTwo" />
        <cards :name="cardNameThree" :amount="cardAmountThree" />
        <cards :name="cardNameFour" :amount="cardAmountFour" />
      </div>

      <div class="experts-container">
        <p>Trusted by experts at</p>
        <img src="../assets/images/experts.svg" alt="" />
      </div>

      <div class="questions-container">
        <h3>Commonly asked questions</h3>
        <p>
          Ship in-app chat messaging with all the features your users expect.
        </p>
        <div class="faqs">
          <faqs :question="cardQuestionOne" :answer="cardAnswerOne" />
          <faqs :question="cardQuestionTwo" :answer="cardAnswerTwo" />
          <faqs :question="cardQuestionThree" :answer="cardAnswerThree" />
          <faqs :question="cardQuestionFour" :answer="cardAnswerFour" />
          <faqs :question="cardQuestionFive" :answer="cardAnswerFive" />
          <faqs :question="cardQuestionSix" :answer="cardAnswerSix" />
          <faqs :question="cardQuestionSeven" :answer="cardAnswerSeven" />
        </div>

        <h4>Got additional questions?</h4>
        <p>We would love to have a chat with you.</p>
        <div class="kemi">
          <button>
            Contact Support <span><img src="../assets/images/blue.svg" /></span>
          </button>
        </div>
      </div>

      <div class="chat-container">
        <div class="chat-left">
          <p>CHAT</p>
          <h3>See the all-in-one chat system in action</h3>
          <p>
            The only tool you will need to power conversations and interactions
            on your product. <b>Go live within days.</b>
          </p>
          <button>
            Start Demo <span><img src="../assets/images/white.svg" /></span>
          </button>
        </div>
        <div class="chat-right">
          <img src="../assets/images/chat.svg" alt="" />
        </div>
      </div>
    </div>
    <!-- <foot /> -->
  </div>
</template>

<script>
import Cards from '../components/cards.vue'
import Faqs from '../components/faqs.vue'
import Foot from '../components/foot.vue'
import navbar from '../components/navbar.vue'
export default {
  name: 'IndexPage',
  components: { navbar, Foot, Cards, Faqs },
  data() {
    return {
      cardNameOne: 'Starter',
      cardAmountOne: '$69',
      cardNameTwo: 'Growth',
      cardAmountTwo: '$389',
      cardNameThree: 'Pro',
      cardAmountThree: '$799',
      cardNameFour: 'Enterprise',
      cardAmountFour: 'Customized',
      cardQuestionOne: 'How is MAU calculated?',
      cardQuestionTwo: 'What happens if I hit my MAU limit?',
      cardQuestionThree: 'What other limits do I need to be aware of?',
      cardQuestionFour: 'How do I purchase higher levels of support?',
      cardQuestionFive: 'What other limits do I need to be aware of?',
      cardQuestionSix:
        'Is every feature automatically included in the enterprise plan?',
      cardQuestionSeven:
        'Do the prices listed on the pricing page include tax?',
      cardAnswerOne:
        'Tax is not included in the prices listed on the pricing page. Tax will be included in your billing receipts.',
      cardAnswerTwo:
        'Tax is not included in the prices listed on the pricing page. Tax will be included in your billing receipts.',
      cardAnswerThree:
        'Tax is not included in the prices listed on the pricing page. Tax will be included in your billing receipts.',
      cardAnswerFour:
        'Tax is not included in the prices listed on the pricing page. Tax will be included in your billing receipts.',
      cardAnswerFive:
        'Tax is not included in the prices listed on the pricing page. Tax will be included in your billing receipts.',
      cardAnswerSix:
        'Tax is not included in the prices listed on the pricing page. Tax will be included in your billing receipts.',
      cardAnswerSeven:
        'Tax is not included in the prices listed on the pricing page. Tax will be included in your billing receipts.',
    }
  },
}
</script>

<style scoped>
.all{
  background: #fff;
   max-width: 1440px;
    margin: 0 auto ;
}
.over-all {
  width: 100%;
  margin: 20px auto 0;
}
.hero-container {
  width: 100%;
  margin: 40px auto;
  text-align: center;
  margin-top: 70px;
  margin-bottom: 40px 0;
}
.hero-container h3 {
  font-weight: 700;
  font-size: 50px;
  margin: 0px auto;
  line-height: 54px;
  padding-top: 20px;
  max-width: 765px;
  text-align: center;
}
.hero-container p {
  font-weight: 400;
  font-size: 20px;
  line-height: 25px;
  opacity: 0.8;
  padding: 30px 0;
}
.hero-container button {
  width: 207px;
  height: 50px;
  background: #4568d1;
  border-radius: 30.5px;
  font-weight: 700;
  font-size: 16px;
  line-height: 20px;
  text-align: center;
  color: #fff;
  margin-bottom: 20px;
  /* padding-right: 10px; */
}
span img {
  margin-left: 20px;
}
.card-container {
  background: blue;
  width: 85%;
  margin: 40px auto;
  display: grid;
  grid-gap: 5px;
  grid-template-columns: 1fr 1fr 1fr 1fr;
    /* display: flex;
  justify-content: space-evenly; */
}
.experts-container {
  width: 100%;
  margin: 40px auto;
  text-align: center;
}
.experts-container img {
  display: block;
  width: 50%;
  margin: 20px auto;
}
.experts-container p {
  font-weight: 700;
  font-size: 15px;
  line-height: 18px;
  opacity: 0.4;
  padding: 20px 0;
}
.faqs {
  margin-bottom: 60px;
  margin: 30px auto;
  /* width: 50%; */
}
.questions-container {
  /* max-width: 100%; */
  background: #f5f7fc;
  border-radius: 25px;

  width: 1238px;
  background: red;
  margin: 40px auto;
  border-radius: 25px;
  padding: 70px 0 0 0;
}
.questions-container h3 {
  font-weight: 700;
  font-size: 35px;
  line-height: 41px;
  text-align: center;
}
.questions-container h4 {
  width: 100%;
  text-align: center;
  padding-top: 20px;
}
.questions-container p {
  font-weight: 400;
  font-size: 19px;
  line-height: 30px;
  width: 362px;
  margin: 0px auto;
  text-align: center;
  opacity: 0.8;
  padding-top: 10px;
}
.kemi{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
 margin: 0 auto;
}
.questions-container button {
  background: #fff;
  border-radius: 30.5px;
  font-weight: 700;
  font-size: 16px;
  line-height: 20px;
  width: 207px;
  height: 50px;
  color: #4568d1;
  margin: 20px auto 50px auto;
}
.chat-container {
  display: flex;
  margin: 30px auto 0;
  width: 100%;
  justify-content: space-between;
}
.chat-left {
  margin-left: 10%;
  padding: 30px 30px;
  margin-top: 100px;
}
.chat-left h3 {
  font-weight: 700;
  font-size: 35px;
  line-height: 41px;
  width: 389px;
  padding: 22px 0 37px 0;
}
.chat-left p {
  font-weight: 400;
  font-size: 19px;
  line-height: 30px;
  opacity: 0.8;
  width: 362px;
}
.chat-left button {
  border: 1px solid #000000;
  font-weight: 700;
  font-size: 16px;
  line-height: 20px;
  width: 207px;
  height: 50px;
  text-align: center;
  color: #333333;
  border-radius: 30.5px;
  margin-top: 87px;
}
.chat-right {
  /* background: blue; */
  position: relative;
}
@media only screen and (max-width: 1200px) {
  .chat-container {
    margin: 20px auto;
  }

  .chat-right {
    display: none;
  }
  .card-container {
    width: 90%;
    grid-gap: 15px;
    grid-template-columns: 1fr 1fr;
  }
  .questions-container {
    width: 90%;
  }
}
@media only screen and (max-width: 600px) {
  .card-container {
    width: 95%;
    grid-template-columns: 1fr;
  }
  .questions-container {
    width: 95%;
  }
  .questions-container p {
    padding: 20px;
  }
  .chat-container {
  display: flex;
  margin: 30px auto 0;
  width: 100%;
  justify-content: space-between;
}
.chat-left {
  margin-left: 10%;
  padding: 30px 30px;
  margin-top: 100px;
}
.chat-left h3 {
  width: 280px;
}
.chat-left p {
  width: 250px;
}
}
</style>
