<template>
  <section class="card" :class="`card--${border}`">

    <div class="card-wrapper">
      <div class="card-username-container">
        <img class="card-image" :src="image" alt="">
        <p class="card-name">{{username}}</p>
      </div>

      <p class="card-number">{{followers}}</p>

      <p class="card-text">{{text}}</p>

      <div class="card-update-container">
        <img class="card-icon" :src="icon" alt="">
        <p class="card-update">{{update}}</p>
      </div>
    </div>

  </section>
</template>

<script>
export default {
  name: 'CardLarge',

  props: {
    image: {
      type: String,
      required: false
    },
    username: {
      type: String,
      required: false
    },
    followers: {
      type: String,
      required: false
    },
    text: {
      type: String,
      required: false
    },
    icon: {
      type: String,
      required: false
    },
    update: {
      type: String,
      required: false
    },
    border: {
      type: String,
      required: false
    },
  }
}
</script>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 230px;
  width: 270px;
  background-color:  #f0f3fa;
  border-top: 4px solid blue;
  border-radius: 5px;

  &-wrapper {
    display: flex;
    justify-content: space-between;
    flex-direction: column;
    align-items: center;
    height: 165px;
  }

  &-image {
    width: 21px;
    height: 21px;
  }

  &-username-container {
    display: flex;
    justify-content: center;
    align-items: center;
  } 

  &-name {
    font-size: 12px;
    color: rgb(154, 154, 154);
  }

  &-number {
    font-size: 44px;
    font-weight: 700;
    color: black;
  }

  &-text {
    font-size: 12px;
    font-weight: 200;
    color: rgb(154, 154, 154);
    text-transform: uppercase;
    letter-spacing: 5px;
  }

  &-update-container {
    display: flex;
    align-items: center;
  }

  &-update {
    font-size: 12px;
    color: green;
  }
}
</style>