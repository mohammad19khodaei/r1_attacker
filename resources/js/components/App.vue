<template>
  <div class="container">
    <nav class="navbar navbar-expand-lg navbar-light" style="background-color: #00BAB9">
      <router-link class="nav-link" :to="{ name: 'home'}">
        <img src="img/r1_1.jpg" alt="" width="45" height="45">
      </router-link>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <router-link class="nav-link" :to="{name: 'addCode'}">Add</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" :to="{name: 'phoneCheck'}">Check</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" :to="{name: 'winnerList'}">List</router-link>
          </li>
          
        </ul>
      </div>
    </nav>
    <router-view></router-view>
  </div>
</template>

<script>
const default_layout = "default";

export default {};
</script>

<style scoped>
.nav-item a {
  color: white !important;
  font-size: 17px;
}

.nav-item a:hover {
  color: gray !important;
}
</style>