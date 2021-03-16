<template>
  <div class="row row-cols-1 row-cols-md-3 g-4">
    <card v-bind:imgURL="imgOne" title="Binding image from root" body="V-bind:imgURL and it gets the image from the root folder by using the @ symbol" />
    <card imgURL="/img/zoltan-tasi-oeo9JeFXPwo-unsplash.jpg" title="Image from new folder under public" body="Created a new img folder under public so I dont need to return the data, I can instead get the image fromt the public/img folder directly." />
    <card imgURL="/img/zoltan-tasi-t8__xN-MdNI-unsplash.jpg" />
</div>
</template>

<script>
import Card from './Card'
export default {
  data() {
    return {
      imgOne: require('@/assets/img/nasa-Q1p7bh3SHj8-unsplash.jpg')
    }
  },
  components: {
    Card
  }
}
</script>

<style>

</style>
