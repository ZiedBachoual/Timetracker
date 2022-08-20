<template>
  <div class="hello">
    <table>
      <tr>
        <th><h1 id="date">Date</h1></th>
        <th><button id="stopbutton">STOP</button></th>
        <th><button id="startbutton">START</button></th>
        <th><h1>Période</h1></th>
      </tr>
    </table>
    <table id="deuxiemetab">
      <tr>
        <td>Period n* </td>
        <td>Date de start</td>
        <td>Durée de periode</td>
      </tr>
      <tr>
        <td></td>
        <td></td>
        <td></td>
        <td>Date totale</td>
      </tr>
    </table>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  name: 'HelloWorld',
  props: {
    message: String
  }
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#date {
     margin-right: 50%;
     margin-top: 5%;
  }
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
#stopbutton{
  color: #f80101;
  margin-top: 10%;
}
#startbutton{
  color: rgb(2, 241, 2);
  margin-top: 10%;
}
table, th, tr{
  display: grid;
  width: 600px;
  grid-template-columns: 120px 120px 120px 120px;
  align-items: start;
  justify-content: space-between;
  margin: auto;
}
#deuxiemetab{
    border: 1px solid black;
}
</style>
