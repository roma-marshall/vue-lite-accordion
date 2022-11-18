<template>
  <div class="flex justify-center bg-gray-500 h-screen py-10">
    <roma-accordion
        :head="head"
        :body="body"
        :darkmode="false"
        :position="position"
    >
    </roma-accordion>
  </div>
</template>

<script>
import RomaAccordion from './components/RomaAccordion.vue'

export default {
  name: 'App',
  components: {
    RomaAccordion
  },
  data() {
    return {
      position: '',
      head: 'FAQ',
      body:
          'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.'
    }
  }
}
</script>

<style>

</style>
