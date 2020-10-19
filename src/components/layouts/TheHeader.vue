<template>
    <header><h1>{{ title }}</h1></header>
</template>

<script>
export default {
    props: ['title']
}
</script>

<style scoped>
header {
  width: 100%;
  height: 5rem;
  background-color: #88b77b;
  display: flex;
  justify-content: center;
  align-items: center;
}

header h1 {
  color: white;
  margin: 0;
  font-weight: 200;
}

@media (min-width: 320px) {
  header h1 {
    font-size: 22px;
  }
}
</style>