<template>
  <div id="sidebar">
    <ul>
      <li>
        <button @click="goTo('home')">Home</button>
      </li>
      <li>
        <button @click="goTo('search')">Search</button>
      </li>
      <li>
        <button @click="goTo('likes')">Likes</button>
      </li>
      <li>
        <button @click="goTo('profile')">Profile</button>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'sidebar',
  methods: {
    goTo (page) {
      this.$router.push(page)
    }
  }
}
</script>

<style>
  #sidebar {
    float: left;
    height: 100%;
    width: 150px;
    background-color: gray;
    text-align: center;
  }

  #sidebar > ul {
    list-style: none;
    margin: 0px;
    padding: 0px;
  }
</style>
