<template>
    <div class="v-basket-item">
          <!-- <p>{{ title }}</p> -->
      <vCatalog />
      <vBasket />
    </div>
</template>
<script>
import vCatalog from './v-catalog.vue'
import vBasket from './v-basket.vue'

export default {
  name: 'v-basket-item',
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

</style>
