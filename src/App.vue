<template>
  <div id="app">
    <Content :listData="data" :itemSize="100">

    </Content>

  </div>
</template>

<script>
import Content from "./components/Content";
let d = [];
for(let i = 0; i < 1000;i++){
  d.push({id:i,value:i})
}
export default {
  name: "App",
  components: {
    Content
  },
  data(){
    return{
      data:d
    }
  },

};
</script>

<style>
html{
  height: 100%;
}
body{
  height: 100%;
  margin:0;
}
#app{
  height:100%;
}
</style>
