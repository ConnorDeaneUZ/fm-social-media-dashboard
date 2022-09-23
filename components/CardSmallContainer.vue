<template>
  <section class="card-container">

    <div class="cards-small" v-for="card in userData" :key="card.number">
      <card-small
       :text="card.text"
       :image="card.image"
       :number="card.number"
       :update="card.update"
       :icon="card.icon"
       />
    </div>

  </section>
</template>

<script>
import userData from '~/config/UserData'
import CardSmall from './CardSmall.vue'

export default {
  name: 'CardContainerSmall',

  components: {
    CardSmall
  },

  data: () => ({
    userData: userData.cardSmallData
  })
}
</script>

<style lang="scss" scoped>
.card-container {
  position: relative;
  display: flex;
}
</style>