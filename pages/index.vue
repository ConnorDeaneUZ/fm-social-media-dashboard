<template>
<section class="container">
  <div class="container-text">
    <h1>Starter Repo</h1>
  </div>
</section>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>


<style lang="scss" scoped>
@import '~/assets/_color-palette.scss';
@import '~/assets/_abstract.scss';


.container {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  height: 110vh;
  width: 100%;
  background-color: colorPaletteSetting(core-grey);
  font-family: abstractSetting(primary_font);

  @media screen and (min-width: 800px ) {
    flex-direction: row;
  }
}

body {
  margin: 0 !important;
  padding: 0 !important;
  box-sizing: border-box !important;
}
</style>