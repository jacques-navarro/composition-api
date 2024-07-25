<template>
  <div class="home">Home</div>
  <p>{{ name }}</p>
  <p>{{ age }}</p>
</template>

<script>
export default {
  name: "HomeView",
  setup() {
    console.log("setup");
    let name = "Jules";
    let age = 7;

    return {
      name,
      age,
    };
  },
};
</script>
