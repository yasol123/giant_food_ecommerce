<template>
    <div class="column is-3">
        <div class="box has-text-centered">
            <figure class="image is-square">
                <router-link v-bind:to="product.get_absolute_url">
                <img v-bind:src="product.get_thumbnail">
                </router-link>
            </figure>
            <h2 class="is-size-6">{{ product.name }}</h2>
            <p class="is-size-6 has-text-grey">${{ product.price }}</p>
            <router-link v-bind:to="product.get_absolute_url" class="button is-dark mt-4">View Details</router-link>
        </div>
    </div>
</template>
<script>

export default{
    name: 'ProductBox',
    props:{
        product: Object
    }
}
</script>
<style scoped>
.image{
    margin-top: -1.25rem;
    margin-left: -1.25rem;
    margin-right: -1.25rem;
}
</style>