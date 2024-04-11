<template>
  <div class="v-catalog-item">
    <img class="v-catalog-item_image" :src="require('../assets/images/' + product_data.image)" alt="picture"/>
    <p class="v-catalog-item_name">{{ product_data.name }}</p>
    <p class="v-catalog-item_price">{{ product_data.price }}</p>
    <p class="v-catalog-item_about">{{ product_data.about }}</p>
    <button class="v-catalog-item__add_to_btn" @click="sendDataToParant">Add to basket</button>
  </div>
</template>
<script>
export default {
  name: 'v-catalog-item',
  props: {
    product_data: {
      type: Object,
      default () {
        return {}
      }
    }
  },
  data () {
    return {}
  },
  methods: {
    sendDataToParant () {
      this.$emit('sendDataToP', this.product_data.article)
    }
  }
}
</script>

<style lang="scss">
.v-catalog-item {
    flex-basis: 25%;
    box-shadow: 0 0 8px 0 grey;
    padding: 20px;
    margin: 20px;
}
</style>
