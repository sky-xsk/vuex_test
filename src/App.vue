<template>
    <div id="app">
        <h3>vuex</h3>
        <Cart></Cart>
        <ProductList></ProductList>
    </div>
</template>

<script>
import Cart from './components/Cart.vue';
import ProductList from './components/ProductList.vue';
import {mapState,mapMutations,mapGetters,mapActions} from 'vuex';
export default {
    data() {
        return {
            
        }   
    },
   
    components: {
        Cart,
        ProductList
    },
}

</script>
<style lang="scss">
#app{text-align: center;}
</style>