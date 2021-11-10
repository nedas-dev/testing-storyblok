<template>
  <div
    v-editable="blok"
    class="py-8 mb-6 text-5xl font-bold text-center">
    <h3>{{ blok.headline }}</h3>
    <img :src="blok.image.filename"/>
    <script>console.log({{ blok.image }})</script>
  </div>
</template>
 
<script>
export default {
  props: {
    blok: {
      type: Object,
      required: true
    }
  }
}
</script>