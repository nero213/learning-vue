<script>
export default{
  data(){
    return {
      username: '',
      showusername: false
    };
  },
  methods:{
    toggleUsername() {
      this.showusername = this.showusername;
    }
    
  }
}

</script>

<template>
 <div>
  <input v-model="username" type="text" placeholder="Enter your username"/>
  <button @click="toggleUsername">Toggle Username</button>
  <p v-if="showusername">Your username is: {{ username }}</p>
  <p v-else>Your username is hidden</p>
    

 </div>

</template>