<template>
    <div class="m-nav">
        <ul class="nav">
            <li class="list">
                <nuxt-link to="/my">我的美团</nuxt-link>
                <dl>
                    <dd><nuxt-link to="/order">我的订单</nuxt-link></dd>
                    <dd><nuxt-link to="/order">我的收藏</nuxt-link></dd>
                    <dd><nuxt-link to="/order">抵用券</nuxt-link></dd>
                    <dd><nuxt-link to="/order">我的设置</nuxt-link></dd>
                </dl>
            </li>
            <li>
                <nuxt-link to="/order">手机App</nuxt-link>
            </li>
            <li class="list bd">
                <nuxt-link to="/center">商家中心</nuxt-link>
                <dl>
                    <dd><nuxt-list to="/userCenter">登录商家中心</nuxt-list></dd>
                    <dd><nuxt-list to="/userCenter">我想合作</nuxt-list></dd>
                    <dd><nuxt-list to="/userCenter">免费手机开店</nuxt-list></dd>
                    <dd><nuxt-list to="/userCenter">商家申请开票</nuxt-list></dd>
                </dl>
            </li>
            <li class="list site">
                <nuxt-link to="/site">网站导航</nuxt-link>
                <div class="subContainer">
                    <dl class="hotel">
                        <dt></dt>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                        <dd>国际机票</dd>
                    </dl>
                     <dl class="food">
                        <dt>美食</dt>
                        <dd>烤鱼</dd>
                        <dd>烤鱼</dd>
                        <dd>烤鱼</dd>
                        <dd>烤鱼</dd>
                        <dd>烤鱼</dd>
                        <dd>烤鱼</dd>
                        <dd>烤鱼</dd>
                        <dd>烤鱼</dd>
                        <dd>烤鱼</dd>
                        <dd>烤鱼</dd>
                    </dl>
                     <dl class="movie">
                         <dt>看电影</dt>
                        <dd>看电影</dd>
                        <dd>看电影</dd>
                        <dd>看电影</dd>
                        <dd>看电影</dd>
                        <dd>看电影</dd>
                        <dd>看电影</dd>
                        <dd>看电影</dd>
                        <dd>看电影</dd>

                    </dl>
                     <dl class="app">
                         <dt>手机应用</dt>
                        <dd>1</dd>
                    </dl>
                </div>
            </li>
        </ul>
    </div>    
</template>
<script>
export default {
    
}
</script>
<style lang="scss">
</style>
