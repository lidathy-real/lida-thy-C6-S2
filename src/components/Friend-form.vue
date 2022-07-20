<template>
  <div class="main">
    <input type="text" placeholder="First Name" id="input" v-model="firstName">
    <input type="text" placeholder="Last Name" id="input" v-model="lastName">
    <input type="text" placeholder="comment" id="input" v-model="comment">
    <button @click="addFriend">Add</button>
  </div>
  <FriendCard
    :friends = "friends"
  />
</template>

<script>
import FriendCard from "./Friend-card.vue";
export default {
    components:{
       FriendCard,
    },
    data(){
      return{
        firstName:'',
        lastName:'',
        comment:'',
        fullName:'',
        friends:[]
      }
    },
    methods:{
      addFriend(){
        this.fullName = this.firstName + ' ' + this.lastName;
        if(this.firstName != '' && this.lastName != '' && this.comment != ''){
          this.friends.push({fullName:this.fullName,comment:this.comment});
          this.firstName = '';
          this.lastName = '';
          this.comment = '';
        }else{
          window.alert("Must be input in the blank! 😎😥");
        }
      }
    }
}
</script>

<style>

</style>