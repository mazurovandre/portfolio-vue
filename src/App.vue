<template>
  <Transition name="slide">
    <main-info :info="state.profile"/>
  </Transition>

</template>

<script>
import json from "./json/data.json"
import MainInfo from "@/components/MainInfo";

export default {
  name: 'App',
  components: {MainInfo},
  setup() {
    const state = json;
    return {
      state
    }
  }
}
</script>

<style lang="sass">

</style>
