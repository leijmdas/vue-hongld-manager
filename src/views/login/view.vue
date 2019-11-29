<template>
 <div>
   <Tabs active-key="key1">
     <Tab-pane label="标签一" key="key1">标签一的内容</Tab-pane>
     <Tab-pane label="标签二" key="key2">标签二的内容</Tab-pane>
     <Tab-pane label="标签三" key="key3">标签三的内容</Tab-pane>
   </Tabs>

   <template>
     <Row>
       <i-col span="12">col-12</i-col>
       <i-col span="12">col-12</i-col>
     </Row>
     <br>
     <Row>
       <i-col span="8">col-8</i-col>
       <i-col span="8">col-8</i-col>
       <i-col span="8">col-8</i-col>
     </Row>
     <br>
     <Row>
       <i-col span="6">col-6</i-col>
       <i-col span="6">col-6</i-col>
       <i-col span="6">col-6</i-col>
       <i-col span="6">col-6</i-col>
     </Row>
   </template>


   <i-button>Default</i-button>
   <i-button type="primary">Primary</i-button>
   <i-button type="ghost">Ghost</i-button>
   <i-button type="dashed">Dashed</i-button>
   <i-button type="text">Text</i-button>
   <br><br>
   <i-button type="info">信息按钮</i-button>
   <i-button type="success">成功按钮</i-button>
   <i-button type="warning">警告按钮</i-button>
   <i-button type="error">错误按钮</i-button>

   <Menu :theme="theme3" active-key="1">
     <Menu-group title="内容管理">
       <Menu-item key="1">
         <Icon type="document-text"></Icon>
         文章管理
       </Menu-item>
       <Menu-item key="2">
         <Icon type="chatbubbles"></Icon>
         评论管理
       </Menu-item>
     </Menu-group>
     <Menu-group title="统计分析">
       <Menu-item key="3">
         <Icon type="heart"></Icon>
         用户留存
       </Menu-item>
       <Menu-item key="4">
         <Icon type="heart-broken"></Icon>
         流失用户
       </Menu-item>
     </Menu-group>
   </Menu>
   <br>
   <p>切换主题</p>
   <Radio-group :model.sync="theme3">
     <Radio value="light"></Radio>
     <Radio value="dark"></Radio>
   </Radio-group>
 </div>
</template>

<script>
import axios from 'axios';

export default {
  data() {
    return {
      msg: 'Hello worldcom!'
    }
  },
  methods:{
    demo (){

    }
  }
}
</script>

<style scoped>
  .red {
    color: #f00;
  }
</style>
