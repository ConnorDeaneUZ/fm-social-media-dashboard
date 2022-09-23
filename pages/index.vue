<template>
<section class="container">

  <primary-nav />

  <card-large-container />

  <card-small-container />

</section>
</template>

<script>
import PrimaryNav from '../components/PrimaryNav.vue'
import CardLargeContainer from '../components/CardLargeContainer.vue'
import CardSmall from '../components/CardSmall.vue'
import CardSmallContainer from '../components/CardSmallContainer.vue'

export default {
  name: 'IndexPage',

  components: {
    PrimaryNav,
    CardLargeContainer,
    CardSmall,
    CardSmallContainer
  }
}
</script>

<style lang="scss">
@import '~/assets/_color-palette.scss';
@import '~/assets/_abstract.scss';

.container {
  font-family: abstractSetting(primary_font);
  // height: 100vh;
}

body {
  margin: 0 !important;
  padding: 0 !important;
  box-sizing: border-box !important;
}

* {
  margin: 0;
  padding: 0;
}
</style>