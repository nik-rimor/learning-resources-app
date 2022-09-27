<template>
  <ul>
    <li v-for="resource in storedResources" :key="resource.id">
      <h2>{{ resource.title }}</h2>
      <p>{{ resource.description }}</p>
    </li>
  </ul>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      storedResources: [
        {
          id: "official-guide",
          title: "Official Guide",
          description: "The Official Vue.js documentation.",
          link: "https://vuejs.org",
        },
        {
          id: "google",
          title: "Google",
          description: "Learn to google...",
          link: "https://google.org",
        },
      ],
    };
  },
};
</script>

<style lang="scss"></style>
