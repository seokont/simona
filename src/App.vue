<template>
  <div id="app">
    <router-link to="/"></router-link>

    <router-view/>
  </div>
</template>
<script>
import Home from "@/components/Home";
export default {
  comments: {Home}
}
</script>


