<template>
  <the-header title="RememberMe" />
  <stored-resource :resources="storedResources" />
</template>

<script>
import StoredResource from './components/learning-resource/StoredResource.vue';
import TheHeader from './components/layouts/TheHeader.vue';

export default {
  components: {
    StoredResource,
    TheHeader,
  },
  data() {
    return {
      storedResources: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official Vue.js documentation',
          link: 'https://vuejs.org',
        },
        {
          id: 'vue-school',
          title: 'Vue School',
          description: 'The best Vue.js video courses',
          link: 'https://vueschool.io',
        },
        {
          id: 'vue-mastery',
          title: 'Vue Mastery',
          description: 'The ultimate learning resource for Vue.js developers',
          link: 'https://www.vuemastery.com',
        },
      ],
    };
  },
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>
