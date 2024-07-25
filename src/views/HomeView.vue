<template>
  <div class="home">Home</div>
  <p>{{ name }}</p>
  <p>{{ age }}</p>
  <button @click="handleClick">Click Me!</button>
</template>

<script>
export default {
  name: "HomeView",
  setup() {
    console.log("setup");
    let name = "Jules";
    let age = 7;

    const handleClick = () => {
      console.log("Clicked!");
    };

    return {
      name,
      age,
      handleClick,
    };
  },
};
</script>
