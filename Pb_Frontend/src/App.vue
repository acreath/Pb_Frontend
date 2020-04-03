<template>
  <div id="app">
    
    <div class="layout">
        <Layout>
            <Header>
                <Menu mode="horizontal" theme="light" active-name="1">
                    <div class="layout-logo">
                      <img src="./assets/logo.png" style="height:40px; width:140px">
                    </div>
                    <div class="layout-nav">
                        <MenuItem name="1">
                            <Icon type="ios-navigate"></Icon>
                            首页
                        </MenuItem>
                        <Submenu name="2">
                            <template slot="title">
                                <Icon type="ios-stats" />
                                入门学习
                            </template>
                            
                            <MenuItem name="2-1"> 标准流程</MenuItem>
                            <MenuItem name="2-2">规范文档</MenuItem>
                            <MenuItem name="2-3">基础技术</MenuItem>    
                           
  
                        </Submenu>
                        <MenuItem name="3">
                            <Icon type="ios-analytics"></Icon>
                            能力训练
                        </MenuItem>
                        <Submenu name="4">
                            <template slot="title">
                                <Icon type="ios-stats" />
                                 信息广场
                            </template>
                            
                            <MenuItem name="4-1">领域信息</MenuItem>
                            <MenuItem name="4-2">经验分享</MenuItem>
                            <MenuItem name="4-3">思维模型</MenuItem>    
                           
  
                        </Submenu>
                    </div>
                    <div class="layout-login">
                      <Avatar icon="ios-person" />
                      <span>{{usrname}}</span>
                    </div>
                </Menu>
            </Header>
            <Content :style="{padding: '0 50px'}">
                <router-view/>
            </Content>
            
            <Footer class="layout-footer-center">2011-2022 &copy; ProductBoard</Footer>
        </Layout>
    </div>
     
    
    
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
                theme1: 'light',
                usrname: '登录/注册'
            }
  }
}
</script>

<style scoped>
.ivu-layout-header{
  background: white;
  padding: 0px;
}

.layout{
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    border-radius: 4px;
    overflow: hidden;
}
.layout-logo{
    width: 140px;
    height: 30px;
    background: #5b6270;
    border-radius: 3px;
    float: left;
    position: relative;
    top: 10px;
    left: 300px;
    
}
.layout-nav{
    width: 620px;
    margin: 0 auto;
    /* margin-right: 20px; */
    float: left;
    margin-left:30% ;
}
.layout-footer-center{
    text-align: center;
}
.layout-login{
    margin:auto 0;
    height: 30px;
    
}
</style>
