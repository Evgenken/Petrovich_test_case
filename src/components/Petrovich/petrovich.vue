<template>
  <div class="qwer">
    <div class="qwer__asdf">asdfasdf</div>
    <div  class="qwer" v-for="(item, key) in qwer" :key="key">
      <petrovich-card :text="item" />
    </div>
  </div>
</template>

<script>
import PetrovichCard from '@/components/Petrovich/petovich-card.vue';
export default {
  name: 'Petrovich',
  components: {PetrovichCard},

  data() {
    return {
      qwer: [
        {name: 'Evgen', titul: 'huevii', prof: 'electrik' },
        {name: 'Arsd', titul: 'Luch', prof: 'Code' },
        {name: 'Mih', titul: 'middle', prof: 'Test' }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
.qwer {
  width: 100%;
  background: red;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 200px;
  flex-wrap: wrap;

  &__asdf {
    background: green;
    width: 50%;
    height: 100px;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}

</style>
