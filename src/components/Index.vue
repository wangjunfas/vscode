<template>
    <div id="header" >
        <div class="box">
            <h1 class="head-left" @click="showList">
                <a>
                    <div class="iconfont icon-caidan"></div>
                    <div class="maizuo">卖座电影</div>
                </a>
            </h1>
            <div class="head-right">
                <router-link to="/city" tag="a" class="city">
                    <span>北京</span>
                    <i class="iconfont icon-xia"></i>
                </router-link>
                <router-link to="/login" tag="a" class="iconfont icon-wode"></router-link>
            </div>
        </div>
        <transition-group>
          
        </transition-group>



    </div>
    

    
    

</template>

<script>

export default {
  name: 'Index',
  data () {
    return {
      arr:["首页","影片","影院","商城","我的","卖座卡"],
      isShow:true

    }
  },
  methods:{
    showList(){
      alert("1111")
    }
  }
}
</script>

<style lang="scss" scoped>
    .box{
      background: #282828;
      position: fixed;
      z-index: 500;
      top: 0;
      right: 0;
      left: 0;
      width: auto;
      height: 50px;
      line-height: 50px;
      overflow: hidden;
    }
    .head-left{
      color: #fff;
      font-size: 16px;
      line-height: 50px;
      text-align: left;
      text-shadow: 0 -1px 0 rgba(0,0,0,0.8);
      width: auto;
      height: 50px;
      margin: 0 auto;
      float: left;
    }
    .icon-caidan{
      float:left;
      width:48px;
      text-align: center;
      color: #999;
      border-right:1px solid #222;
      box-shadow: 1px 0 1px #363636;
    }
    .maizuo{
      float:left;
      text-align: center;
      padding:0 1em;
      font-weight:600;
      color:#fff;
      
    }
    .head-right{
      color:#999;
      width:105px;
      height:50px;
      float:right;
      text-align:center;
      .city{
        //color:#999;
        float: left;
        font-size: 14px;
        padding: 0 6px;
        .icon-xia{
          //color:#999;
          font-size:12px;
          font-weight:600;
        }
      }
      .icon-wode{
        float: left;
        font-size: 16px;
        width: 48px;
        font-weight:600;
        color:#999;
      }
    }
</style>

