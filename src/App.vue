<template id="Test">
  <head>
    <title>TEST 2</title>
  </head>
  <body>
  <nav>
  <div class="logo">
    <span class="name_logo">TEST 1-2</span>
  </div>
  </nav>
    <div class="carousel" id="app">
      <Slider />
    </div>
  <div class="data-names">
    <table>
      <tr>
        <th><div v-on:click="sortParam='ID'">ID</div></th>
        <th><div v-on:click="sortParam='Name'">Имя</div></th>
        <th><div v-on:click="sortParam='Data'">Дата рождения</div></th>
        <th><div v-on:click="sortParam='Price'">Цена</div></th>
      </tr>
      <tr>
        <td>id:0001</td>
        <td>Артём Борисов</td>
        <td>2001-02-12</td>
        <td>1000</td>
      </tr>
      <tr>
        <td>id:0002</td>
        <td>Егор Данилюк</td>
        <td>2001-27-07</td>
        <td>2000</td>
      </tr>
      <tr>
        <td>id:0003</td>
        <td>Кирилл Поздеев</td>
        <td>3000-02-15</td>
        <td>Бесценно</td>
      </tr>
      <tr>
        <td>id:0004</td>
        <td>Человек 1</td>
        <td>2001-02-12</td>
        <td>1000</td>
      </tr>
      <tr>
        <td>id:0005</td>
        <td>Человек 2</td>
        <td>2001-02-12</td>
        <td>1000</td>
      </tr>
    </table>
  </div>
  </body>
</template>
<script>
import Slider from "./components/Slider.vue";
export default {
  name: "app",
  components: {
    Slider
  }
};
</script>
<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  margin: 0px;
}
table {
  border-collapse: collapse;
  line-height: 1.1;
  background: gainsboro;
  color: black;
}
th {
  padding: 20px;
  border: 1px solid dimgray;
}
td {
  font-size: 16px;
  padding: 10px 10px;
  border: 1px solid dimgray;
}
</style>