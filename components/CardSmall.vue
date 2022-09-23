<template>
  <section class="card">
    <div class="card-upper">
      <p class="card-text">{{text}}</p>
      <img class="card-image" :src="image" alt="">
    </div>
    <div class="card-lower">
      <p class="card-number">{{number}}</p>

      <div class="card-update-container">
        <img :src="icon" alt="">
        <p class="card-update">{{update}}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'CardSmall',

  props: {
    text: {
      type: String,
      required: false
    },
    image: {
      type: String,
      required: false
    },
    number: {
      type: String,
      required: false
    },
    update: {
      type: String,
      required: false
    },
    icon: {
      type: String,
      required: false
    }
  }
}
</script>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  width: 270px;
  height: 132px;
  border-radius: 5px;
  background-color:  #f0f3fa;
  margin: 10px;

  &-text {
    color: gray;
    font-size: 14px;
    font-weight: 500;
  }

  &-number {
    font-size: 32px;
    font-weight: 700;
  }

  &-update {
    font-size: 12px;
    color: green;
  }

  &-upper {
    padding: 20px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  &-lower {
    padding: 20px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  &-update-container {
    display: flex;
    align-items: center;
  }
}
</style>