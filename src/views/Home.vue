<template>
  <div class="l-page home">
    <div class="l-inner">
      <h1 class="home__logo c-logo"><img src="@/assets/images/logo.png" alt=""></h1>
      <div class="home__lead c-lead">
        <p>ホラー映画に詳しくなれる10問を用意しました。日本映画から3問、海外映画から7問出題します。</p>
        <p>最新作から古典的名作まで、幅広く出題しています。興味を持った映画があれば、これを機に観てみてください。中にはシャレにならないくらい怖い作品もあるので、自己責任でどうぞ。</p>
      </div>

      <p class="home__btn c-btn"><router-link to="/question">クイズに挑戦する</router-link></p>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Home',
  components: {
  },
});
</script>
<style lang="scss" scoped>
  .home {
    padding: 50px 0 0;
    &__lead {
      margin-top: 38px;
    }
    &__btn {
      margin-top: 40px;
    }
  }
</style>
