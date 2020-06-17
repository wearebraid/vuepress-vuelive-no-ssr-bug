<template>
  <ul>
    <li
      v-for="(value, key) in items"
      :key="key"
    >
     {{ key }}: {{ value }}
    </li>
  </ul>
</template>

<script>
export default {
  props: {
    items: {
      type: Object,
      required: true
    }
  }
}
</script>

<style>
ul {
  border: 1px solid gray;
  padding: 2em;
}
</style>