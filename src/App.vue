<template>
  <div id="app" @after-enter="openTop()">
    <router-view />

    <!-- vue snotify alert -->
    <vue-snotify />
  </div>
</template>

<script>
export default {
  name: "App",
  methods: {
    openTop() {
      console.log("test");
    }
  }
}
</script>