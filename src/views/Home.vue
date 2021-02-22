<template>
  <div class="home">
    <FileUploader msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import FileUploader from '@/components/FileUploader.vue'

export default {
  name: 'Home',
  components: {
    FileUploader
  }
}
</script>
