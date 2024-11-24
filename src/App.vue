<script>

</script>

<template>
  <div class="container">
    <h1>BotB4mbolbi</h1>
    <h2>Platform: {{ TWA.platform }}</h2>
    <h2>Name: {{ TWA.initDataUnsafe.user.first_name}}</h2>
    <h2>Username: {{ TWA.initDataUnsafe.user.username }}</h2>
    <h2>ID: {{ TWA.initDataUnsafe.user.id }}</h2>
    <h2>Language: {{ TWA.initDataUnsafe.user.language_code }}</h2>

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