<template>
  <div class="l-page answer">
    <header class="l-header">
      <h1 class="l-header__logo c-logo"><img src="@/assets/images/logo.png" alt=""></h1>
    </header>
    <div class="l-inner">

      <div class="answer__box c-box">
        <p class="answer__correct answer__correct--is-correct"><img src="@/assets/images/img_correct.png" alt="正解"></p>
        <dl class="answer__txt">
          <dt>A.<b>テレビ</b></dt>
          <dd>1998年に公開され、日本のホラーブームの火付け役となった映画『リング』。見た者が1週間後に死んでしまう「呪いのビデオ」が題材です。特に有名なのは、怨霊の「貞子」が大学講師の高山を襲うシーン。テレビの映像で井戸の中から現れ、テレビから這い出てくる姿は、多くの観客に恐怖を与えました。</dd>
        </dl>
      </div>

      <p class="answer__btn c-btn"><router-link to="/question">次の問題へ</router-link></p>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'answer',
  components: {
  },
});
</script>
<style lang="scss" scoped>
  .answer {
    &__correct {
      margin: 0 auto;
      &--is-correct {
        width: percentage(215/630);
      }
      &--is-incorrect {
        width: percentage(193/630);
      }
    }
    &__txt {
      margin-top: 15px;
      dt {
        font-weight: 700;
        font-size: 1.6rem;
        b {
          color: #870006;
          font-size: 2.1rem;
          display: inline-block;
          margin-left: 5px;
        }
      }
      dd {
        font-size: 1.3rem;
        line-height: 2;
      }
    }
    &__btn {
      margin-top: 40px;
    }
  }
</style>
