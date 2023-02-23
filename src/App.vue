<template>
  <LearningResource
    v-for="res in storedResources"
    :key="res.id"
    :title="res.title"
    :description="res.description"
    :link="res.link"
  />
</template>

<script>
import LearningResource from './components/learning-resources/LearningResource.vue'

export default {
  components: {
    LearningResource
  },
  data () {
    return {
      storedResources: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official Vue.js documentation.',
          link: 'https://vuejs.org'
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Learn to Google...',
          link: 'https://google.org'
        }
      ]
    }
  }
}
</script>
