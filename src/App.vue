<script>
export default {
  data() {
    return {
      name: TWA.initDataUnsafe.user.first_name,
      username: TWA.initDataUnsafe.user.username,
      id: TWA.initDataUnsafe.user.id,
      language: TWA.initDataUnsafe.user.language_code,
      photo: TWA.initDataUnsafe.user.photo,
      platform: TWA.platform
    }
  }

}

</script>

<template>
  <div class="container">
    <h1>BotB4mbolbi</h1>
    <h2>Platform: {{ platform }}</h2>
    <h2>Name: {{ name }}</h2>
    <h2>Username: {{ username }}</h2>
    <h2>ID: {{ id }}</h2>
    <h2>Language: {{ language }}</h2>
    <h2>Photo: {{ photo }}</h2>
  </div>

</template>

<style scoped>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}
.container{
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background-color: #f5f5f5;
  color: #333;

}

</style>