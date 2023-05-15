<script>
import TestComponent from './components/icons/TestComponent.vue'
import TombolTwo from './components/icons/TombolTwo.vue'
export default {
  data() {
    return {
      pesan: '.. hello kalian'
    }
  },
  components: {
    TestComponent,
    TombolTwo
  }
}
</script>

<template>
  <div>
    <TestComponent />
    <TombolTwo />
  </div>
  <div class="display">
    <h2>Testing view ajakn tie</h2>
    <h2>{{ pesan }}</h2>
  </div>
  <div>
    <h2>Testing list</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam quis voluptate ea sapiente
      sit dicta ratione, quibusdam, ut perferendis esse cupiditate delectus quisquam dolor alias
      nemo reprehenderit amet. Ratione, aspernatur.
    </p>
    <ul>
      <li>data</li>
      <li>data</li>
      <li>data</li>
      <li>data</li>
      <li>data</li>
      <li>data</li>
      <li>data</li>
    </ul>
  </div>
</template>

<style>
h2,
.color {
  color: green;
  text-align: center;
}
.display {
  display: flex;
  justify-content: space-around;
  border: solid black 1px;
}
</style>
