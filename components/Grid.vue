<template>
  <ul
    v-editable="blok"
    class="flex py-8 mb-6">
    <li
      v-for="blok in blok.columns"
      :key="blok._uid"
      class="flex-auto px-6">
      <component 
        :is="blok.component"
        :blok="blok" />
    </li>
  </ul>
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