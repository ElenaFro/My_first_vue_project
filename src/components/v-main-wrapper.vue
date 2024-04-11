<template>
  <div class="v-main-wrapper">
        <!-- <p>{{ title }}</p> -->
    <vCatalog />
    <vBasket />
  </div>
</template>

<script>
import vCatalog from './v-catalog.vue'
import vBasket from './v-basket.vue'

export default {
  name: 'v-main-wrapper',
  components: { vCatalog, vBasket },
  props: {},
  data () {
    return {
      title: 'hello!'
    }
  },
  computed: {},
  methods: {},
  watch: {},
  created () {},
  mounted () {
    console.log("hello i'm here")
  }
}
</script>

<style>
.v-main-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  max-width: 900px;
  margin: 0 auto;
}
</style>
