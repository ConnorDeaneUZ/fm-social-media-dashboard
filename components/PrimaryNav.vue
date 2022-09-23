<template>
  <section class="nav">

    <div class="nav__header">
      <p class="nav__heading">Social Media Dashboard</p>
      <p class="nav__followers">Total Followers: 23,004</p>
    </div>

    <div class="nav__toggle">
      <button>Toggle</button>
    </div>
  </section>
</template>

<script>
export default {
  name: 'PrimaryNav'
}
</script>

<style lang="scss" scoped>
.nav {
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  height: 254px;
  // max-width: 1440px;
  // padding: 40px 25px 0 25px;
  background-color: #f8f9fe;

  @media screen and (min-width: 800px ) {
    flex-direction: row;
    // padding: 0 135px;
  }

  &__header {
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 50%;
    border-bottom: 1px solid black;

    @media screen and (min-width: 800px ) {
      border: none;
    }
  }

  &__heading {
    font-size: 26px;
    font-weight: 700;
    padding: 0;
    margin: 0;
  }

  &__followers {
    font-size: 13px;
    font-weight: 400;
    color: rgb(154, 154, 154);
    padding: 0;
    margin: 0;
  }

  &__toggle {
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 50%;
  }
}
</style>