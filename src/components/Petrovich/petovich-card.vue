<template>
  <div class="card">
    <div class="card__name">{{text.name}}</div>
    <div class="card__titul">{{text.titul}}</div>
    <div class="card__prof">{{ text.prof }}</div>
  </div>
</template>

<script>
export default {
  name: 'PetrovichCard',

  props: {
    text: {
      type: Array,
      default: ()=> []
    }
  }
}
</script>

<style scoped lang="scss">
.card {
  border: 1px solid white;
  padding: 10px;
  width: 100%;

  &__name {
    color: white;
    text-align: center;
  }

  &__titul {
    color: white;
    text-align: right;
  }

  &__prof {
    color: white;
    text-align: left;
  }
}

</style>
