<script>
export default {
  data() {
    return {
      count: 0
    }
  }
}
</script>

<template>
  <div>
    <button @click="count++">Tombol satu: {{ count }}</button>
  </div>
</template>

<style>
button {
  font-weight: bold;
}
</style>
