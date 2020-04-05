<template>
  <div>
    <sample :title="indexTitle">
      <div class="come">
        slot example
      </div>
      <div slot="named">named slot!!</div>
    </sample>
    <nuxt-link to="/about">ABOUT</nuxt-link>
  </div>
</template>

<script>
import Sample from '~/components/Sample.vue'

export default {
  components: {
    Sample
  },
  data() {
    return {
      indexTitle: 'DefaultTitle'
    }
  }
}
</script>

<style></style>
