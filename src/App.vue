<template>
  <z-canvas :views="$options.components" />
</template>
<script>
export default {
  components: {
    home: () => import('./demo/home'),
    docs: () => import('./demo/docs'),
    hakkimizda: () => import('./demo/hakkimizda'),
    setting: () => import('./demo/setting'),
    scenes: () => import('./demo/scenes'),
    family: () => import('./demo/family'),
    rooms: () => import('./demo/rooms'),
    devices: () => import('./demo/devices'),
    status: () => import('./demo/status')
  },
  mounted () {
    this.$zircle.config({
      debug: true,
      style: {
        theme: 'blue'
      }
    })
    this.$zircle.setView('home')
  }
}
</script>
<style>
  @import url('https://fonts.googleapis.com/css?family=Source+Sans+Pro:400,700');
  @import url('https://use.fontawesome.com/releases/v5.3.1/css/all.css');
</style>
