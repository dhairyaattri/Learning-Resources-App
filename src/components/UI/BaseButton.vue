<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['mode']
}
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: #88b77b;
  border: 1px solid #88b77b;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: #88b77b;
  border-color: #88b77b;
}

.flat {
  background-color: transparent;
  color: #88b77b;
  border: none;
}

.flat:hover,
.flat:active {
  background-color:white;
}
</style>