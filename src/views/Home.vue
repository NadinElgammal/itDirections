<template>
  <section>
    <h1>Home</h1>
    <span>{{ name + age }}</span>
  </section>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      name: "mohamed",
      age: 25,
    }
  },
  mounted() {
    setTimeout(() => {
      this.age = 30;
    }, 5000);
  },
  updated() {
    this.logName();
  },
  methods: {
    logName() {
      console.log("my name is : ", this.name);
    }
  }
}
</script>

<style lang="scss" scoped>
  h1 {
    color: #f00;
  }
</style>