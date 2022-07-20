<template>
  <FriendMenu/>
  <FriendForm/>
  <FriendCard/>
  
</template>

<script>
import FriendMenu from "./components/Friend-nav.vue";
import FriendForm from"./components/Friend-form.vue";
import FriendCard from "./components/Friend-card.vue";

export default {
  components: {
    FriendMenu,
    FriendForm,
    FriendCard,
  }
  }
 
 
</script>

<style>
#app{
  font-family: sans-serif;
  border:2px solid rgb(223, 89, 111);
  width:50%;
  border-style: dashed;
  margin: auto;
  padding: 20px;
  border-radius: 10px;
}
.menu{
  display: flex;
  align-items: center;
  width: 95%;
  height: 5vh;
  background: rgb(223, 89, 111);
  padding: 5px;
  margin: 10px;
}
.menu:hover{
  background: purple;
}
ul{
  width: 50%;
  display: flex;
  justify-content: space-evenly;
}
li {
  list-style: none;
}
a{
  text-decoration: none;
  color:white;
  font-weight: bold;
}
.main, .card{
  width:60%;
  margin: auto;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  margin-top: 10px;
  border-radius: 10px;
}
.card{
  padding: 5px;
  font-family: sans-serif;
}
#input{
  width: 92%;
  padding: 8px;
  margin: 7px;
}
#input:hover{
  background:rgba(128, 0, 128, 0.278);
}
button{
    padding:12px;
    margin: 10px;
    width: 96%;
    background: rgba(93, 89, 89, 0.948);
    color: white;
    font-weight: bold;
    border-radius: 5px;
    border: none;
    font-size:17px;
}
button:hover{
  background: purple;
}

</style>
