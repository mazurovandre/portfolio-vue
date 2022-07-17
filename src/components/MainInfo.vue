<template>
  <section class="section">
    <div class="photo">
      <img src="../assets/avatar.jpg" alt="photo">
    </div>
    <div class="info">
      <h1>{{ info.name }}</h1>
      <h2>{{ info.title }}</h2>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainInfo",
  props: {
    info: Object
  }
}
</script>

<style scoped lang="sass">
.section
  display: flex
  align-items: center
  width: 60vw
  margin: 0 auto
  position: absolute
  top: 50%
  left: 50%
  transform: translate(-50%, -50%)
.photo
  width: 200px
  height: 200px
  margin-right: 50px
  box-shadow: 0 0 10px rgb(0 0 0 / 70%)
  border-radius: 20px
  overflow: hidden
  img
    width: 100%
    height: auto
    object-fit: cover
</style>