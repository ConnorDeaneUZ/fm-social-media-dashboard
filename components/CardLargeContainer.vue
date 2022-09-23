<template>
  <section class="card-container">

  <div class="cards-large" v-for="card in userData" :key="card.followers">
    <card-large 
    :image="card.image"
    :username="card.username"
    :followers="card.followers"
    :text="card.text"
    :icon="card.icon"
    :update="card.update"
    :border="card.border"
    />
  </div>

  </section>
</template>

<script>
import CardLarge from '~/components/CardLarge.vue'
import userData from '~/config/UserData'

export default {
  name: 'CardContainerLarge',

  components: {
    CardLarge
  },

  data: () => ({
    userData: userData.cardLargeData
  })
}
</script>

<style lang="scss" scoped>
.card-container {
  position: relative;
  top: -50px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  height: 100%;
  max-width: 1440px;
  padding: 0;

  @media screen and (min-width: 800px ) {
    flex-direction: row;
    padding: 0 135px;
    top: -115px;
    align-items: flex-start;
  }
}
</style>