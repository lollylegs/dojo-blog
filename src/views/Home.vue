<template>
  <div class="home">
      <h1>home</h1>
      <PostList :posts="posts" />     
  </div>
</template>

<script>
import PostList from '../components/PostList.vue'
import { ref  } from "vue"


export default {
  name: 'Home',
  components: { PostList },
  setup() {
    const posts = ref([
      {title: 'welcome to the blog', body: 'Exercitation est et eiusmod voluptate deserunt eu duis nulla occaecat Lorem. Sunt tempor irure sunt cillum elit occaecat mollit. Aliquip proident est aliqua irure aliquip anim dolore in irure nulla non enim ipsum. Amet deserunt culpa dolor sunt laboris pariatur do incididunt commodo excepteur sit ullamco.', id: 1},
      {title: 'top 5 css tips', body: 'Cillum anim sint nulla quis incididunt.', id: 2},
    ])

     return { posts }
   }  
}
    
</script>



