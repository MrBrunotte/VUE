<template>
    <div class="card h-100">
        <!-- v-bind:src is the same as :src -->
      <img v-bind:src="imgURL" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">{{ title }}</h5>
        <p class="card-text">{{ body }}</p>
      </div>
    </div>
</template>

<script>
export default {
    // This is another way but just with properties and no body using an Array
    //props: ['imgURL', 'title', 'body']

    props: {
        imgURL: {
            type: String,
            required: false,
            default: '...'
        },
        title: {
            type: String,
            required: false,
            default: 'Default Title from props'
        },
        body: {
            type: String,
            required: false,
            default: 'Bodytext from the props object default! Only the image path in the CardDeck img attribute!'
        }
    }
}
</script>

<style>

</style>
