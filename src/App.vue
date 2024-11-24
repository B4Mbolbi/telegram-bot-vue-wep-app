<script>
export default {
  data() {
    return {
      name: 'App'
    }
  }

}

</script>

<template>
  <div>
    <img :src="TWA.initDataUnsafe.user.photo_url">
  </div>
  <div style="width: 100%; height: 100%;background: #008CBA">
    <b>viewportHeight</b>: {{ TWA.viewportHeight }} <br>
    <b>viewportStableHeight</b>: {{ TWA.viewportStableHeight }} <br>

    <h3>Data received</h3>
    <b>initData</b>: {{ TWA.initData }} <br>
    <b>initDataUnsafe</b>: <pre>{{ TWA.initDataUnsafe }}</pre><br>
    <b>platform</b>: <pre>{{ TWA.platform }}</pre><br>
  </div>

</template>