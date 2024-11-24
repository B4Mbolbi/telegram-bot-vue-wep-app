<script>
import Settins from './components/settings.vue'
export default {
  data() {
    return {
      name: 'App'
    }
  },
  components: {
    Settins
  }

}

</script>

<template>
  <div>{{name}}</div>
  <b>initData</b>: {{ TWA.initData }} <br>
  <Settins></Settins>
</template>