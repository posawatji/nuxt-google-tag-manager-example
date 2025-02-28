<template>
  <div class="wrapper">
    <header>
      <button class="download" @click="downloadFile">Download</button>
    </header>
    <div class="container">
      <p>
        Welcome to our website! Here you can find various resources and download
        useful files.
      </p>
    </div>
    <footer>
      <button class="download" @click="downloadFile">Download</button>
    </footer>
  </div>
</template>

<script setup>
const downloadFile = () => {
  alert("Downloading file...");
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
  text-align: center;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}
.wrapper {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}
header {
  background-color: #333;
  color: white;
  padding: 10px;
}
.container {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 20px;
}
footer {
  background-color: #333;
  color: white;
  padding: 10px;
  width: 100%;
  text-align: center;
  margin-top: auto;
}
button {
  padding: 10px 20px;
  font-size: 16px;
  margin: 10px;
  cursor: pointer;
  border: none;
}
.download {
  background-color: #007bff;
  color: white;
  border-radius: 5px;
  transition: background-color 0.3s;
}
.download:hover {
  background-color: #0056b3;
}
</style>
