<template>
  <div class="Profile">
    <h1>This is a profile page{{$route.params.id}}</h1>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'profile',
  components: {
    //HelloWorld
  },
};
</script>
