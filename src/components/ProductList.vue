<template>
  <div class="pro">
    <ul>
      <li v-for="p in allProducts" :key="p.number">
        {{ p.title }} - {{ p.price }}
      </li>
    </ul>
  </div>
</template>

<script>
  import { mapGetters,mapActions} from 'vuex'
  export default {
    computed: {
      ...mapGetters(['allProducts']),
    },
    created() {
      this.$store.dispatch('getAllProducts');
    }
  }
</script>
