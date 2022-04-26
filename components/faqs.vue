<template>
  <div class="container">
    <div class="hy" :class="showAnswerDetails ? 'clicked-div' : ''">
      <br />
      <div class="clickable-div" @click="showAnswer">
        <div class="text">
          <p class="">{{question}}</p>
        </div>
        <div class="icon-div">
          <img :src="`/${arrow}`" alt="" width="11px" height="auto" />
        </div>
      </div>

      <div v-show="showAnswerDetails" class="answer">
        <p> {{answer}}
        </p>
        <br />
      </div>
    </div>
  </div>
</template>

<script>
export default {
   name: 'faqs',
  props: {
    question: String,
    answer: String,
  },
  data() {
    return {
      showAnswerDetails: false,
      arrow: 'up.svg',
      imgSrc: '',
    }
  },
  methods: {
    showAnswer() {
      this.showAnswerDetails = !this.showAnswerDetails
      if (this.arrow === 'up.svg') {
        this.arrow = 'down.svg'
      } else {
        this.arrow = 'up.svg'
      }
    },
  },
}
</script>

<style scoped>
.container {
  background: #fff;
  margin: 0px auto;
  padding: 10px 15px;
  margin-top: 30px;
}
.clicked-div {
  /* padding-bottom: 10vh; */
}
.clickable-div {
  display: flex;
  justify-content: space-between;
  align-items: center;
  cursor: pointer;
  width: 100%;
}
.text p {
  font-weight: 700;
  font-size: 20px;
  line-height: 23px;
}
.answer {
  margin-top: 47px;
}
.answer p {
  font-weight: 400;
  font-size: 19px;
  line-height: 30px;
  text-align: left;
}
</style>
