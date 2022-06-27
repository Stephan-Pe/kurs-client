<template>
  <div>
    <button @click="loadData">Daten Laden</button>
    <hr>
    <ul>
      <li v-for="post in posts" :key="post.id">{{post.title}}</li>
    </ul>
  </div>
</template>

<script>
// @ is an alias to /src
//import { axios } from "axios";

export default {
  name: 'HomeView',
  data(){
    return{
      posts: [
        {id: 1, title: 'Test'}
      ]
    }
  },
  methods:{
    loadData: function () {
      
    }
  }
}
</script>
