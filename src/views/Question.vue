<template>
  <div class="l-page question">
    <header class="l-header">
      <h1 class="l-header__logo c-logo"><img src="@/assets/images/logo.png" alt=""></h1>
    </header>
    <div class="l-inner">

      <div class="question__box c-box">
        <h2 class="question__ttl">Q.<span>1</span></h2>
        <p class="question__txt">映画『リング』の終盤で、貞子は犠牲者の前に何の中から姿を現した？</p>

        <div class="question__answers">
          <div class="question__answer-item c-btn c-btn--gray"><router-link to="/answer">テレビ</router-link></div>
          <div class="question__answer-item c-btn c-btn--gray"><router-link to="/answer">トイレ</router-link></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'question',
  components: {
  },
});
</script>
<style lang="scss" scoped>
  .question {
    &__ttl {
      font-weight: 700;
      font-size: 1.6rem;
      margin-bottom: 15px;
      line-height: 1;
      span {
        font-weight: 700;
        font-size: 2.1rem;
        color: #870006;
      }
    }
    &__answers {
      margin-top: 25px;
    }
    &__answer-item {
      + .question__answer-item {
        margin-top: 15px;
      }
    }
  }
</style>
