<template>
  <div class="about">
    <h1 v-if="their_name != null">Hello {{ their_name }}, this is an about page</h1>
    <h1 v-else>Hello, this is an about page</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna ali...</p>
  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      their_name: this.$route.params.name
    }
  }
}
</script>