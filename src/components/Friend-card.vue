<template>
  <div class="card" v-for="friend in friends" :key="friend">
    <h4>{{friend.fullName}}</h4>
    <p>{{friend.comment}}</p>
  </div>
</template>

<script>
export default {
    props:["friends"]
}
</script>

<style>

</style>