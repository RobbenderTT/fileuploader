<template>
  <div class="hello">
    <input type="file" @change="onFileSelected">
    <button @click="onUpload">Upload</button>
  </div>
</template>

<script>
export default {
  name: 'FileUploader',
  data(){
    return {
      selectedFile: null,
      image: ''
    }
  },
  props: {
    msg: String
  },
  methods: {
    onFileSelected(event){
      console.log(event);
      this.selectedFile = event.target.files[0];
    },
    onUpload(){
      console.log("clicked");

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
