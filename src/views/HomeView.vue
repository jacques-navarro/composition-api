<template>
  <div class="home">Home</div>
  <p ref="p">My name is {{ name }} and I'm {{ age }} years old.</p>
  <button @click="handleClick">Click Me!</button>
</template>

<script>
import { ref } from "vue";

export default {
  name: "HomeView",
  setup() {
    const p = ref(null);

    console.log("setup");

    let name = "Jules";
    let age = 7;

    const handleClick = () => {
      console.log(p, p.value.innerText);
      p.value.classList.add("test")
      p.value.textContent = "Hello Vue"
    };

    return {
      name,
      age,
      handleClick,
      p,
    };
  },
};
</script>
