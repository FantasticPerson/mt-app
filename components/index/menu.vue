<template>
  <div class="m-menu">
      <div class="nav" @mouseleave="mouseleave()">
          <dt>全部分类</dt>
          <dd @mouseenter="enter" v-for="(item,index) in menu" :key="index">
              <i :class="item.type"/>{{item.name}}<span class="arrow"/>
          </dd>
      </div>
      <div class="detail" v-if="kind" @mouseenter="sover" @mouseleave="sout">
          <template v-for="(item,index) in curDetail.child">
              <div :key="index">
                <h4>{{item.title}}</h4>
                <span v-for="v in item.child">{{v}}</span>
             </div>
          </template>
          
      </div>
  </div>
</template>

<script>

export default {
    data(){
        return {
            kind:'',
            menu:[{
                type:'food',
                name:'美食',
                child:[{
                    title:'美食',
                    child:['代金券','代金券','代金券','代金券']
                }]
            },{
                type:'takeout',
                name:'外卖',
                child:[{
                    title:'美食777',
                    child:['代金券','代金券','代金券','代金券']
                }]
            }]
        }
    },
    computed:{
        curDetail :function(){
            console.log(this.menu.filter((item)=>{
                return item.type == this.kind
            })[0] || [])
            return this.menu.filter((item)=>{
                return item.type == this.kind
            })[0] || []
        }
    },
    methods:{
        mouseleave:function(){
            this.timer = setTimeout(()=>{
                this.kind = ''
            },150)
        },
        enter:function(e){
            console.log(e.target.querySelector('i').className)
            this.kind = e.target.querySelector('i').className
        },
        sover:function(){
            if(this.timer){
                clearTimeout(this.timer)
            }
        },
        sout:function(){
            this.kind = ''
        }
    },
    components: {
    }
};
</script>

<style lang="scss">
</style>

