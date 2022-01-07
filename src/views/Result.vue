<template>
  <div class="l-page result">
    <header class="l-header">
      <h1 class="l-header__logo c-logo"><img src="@/assets/images/logo.png" alt=""></h1>
    </header>
    <div class="l-inner">

      <div class="result__box c-box">
        <h2 class="result__ttl">あなたの正解数</h2>
        <p class="result__num"><b>5</b>/10</p>
        <p class="result__btn c-btn c-btn--gray"><router-link to="/question">TOPへ戻る</router-link></p>
      </div>

    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'result',
  components: {
  },
});
</script>
<style lang="scss" scoped>
  .result {
    &__ttl {
      text-align: center;
      font-size: 2.2rem;
      font-weight: 700;
      color: #d90e0e;
    }
    &__num {
      text-align: center;
      font-size: 2.4rem;
      b {
        font-size: 4.8rem;
         color: #d90e0e;
      }
    }
    &__btn {
      margin: 30px auto 0;
    }
  }
</style>
