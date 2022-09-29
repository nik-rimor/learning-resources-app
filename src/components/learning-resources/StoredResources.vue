<template>
  <ul>
    <learning-resource
      v-for="resource in resources"
      :key="resource.id"
      v-bind="resource"
    >
    </learning-resource>
  </ul>
</template>
<script>
import LearningResource from './LearningResource.vue';

export default {
  name: 'StoredResources',
  inject: ['resources'],
  components: {
    LearningResource,
  },
};
</script>

<style lang="scss" scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
