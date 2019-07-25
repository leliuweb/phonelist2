<template>
  <div id="app">
  <my-header custom-title="通讯录" custom-fixed>
                 <button @touchstart="backBtn" slot="left">返回</button> 
                 <button @touchstart="homeBtn" slot="right">主页</button>   
            </my-header>
            <my-list :user-data="userData"></my-list> 
          </div>
</template>

<script>
  var userData = [
            {"index":"A","users":[
              {"name":"a1","tel":"130111111111"},
              {"name":"a2","tel":"130111111111"},
              {"name":"a3","tel":"130111111111"}
            ]},
            {"index":"B","users":[
              {"name":"b1","tel":"130111111111"},
              {"name":"b2","tel":"130111111111"},
              {"name":"b3","tel":"130111111111"}
            ]},
            {"index":"C","users":[
              {"name":"c1","tel":"130111111111"},
              {"name":"c2","tel":"130111111111"},
              {"name":"c3","tel":"130111111111"}
            ]},
            {"index":"D","users":[
              {"name":"d1","tel":"130111111111"},
              {"name":"d2","tel":"130111111111"},
              {"name":"d3","tel":"130111111111"}
            ]},
            {"index":"E","users":[
              {"name":"e1","tel":"130111111111"},
              {"name":"e2","tel":"130111111111"},
              {"name":"e3","tel":"130111111111"}
            ]}
          ];
export default {
  name: 'app',
  data () {
    return {
      userData: userData
    }
  },
               methods : {
                  backBtn:function(){
                     alert('123');
                  },
                  homeBtn:function(){
                     alert('456');
                  }
                }
}
</script>

<style>
*{margin:0;padding: 0;}
        li{list-style: none;}
        body{}
</style>