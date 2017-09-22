<template>
<div class="content">
    <myheader></myheader>
    <myslogan></myslogan>
    <mytype></mytype>
    <div class="list">
        <mylist></mylist>
        <mylist></mylist>
        <mylist></mylist>
        <mylist></mylist>
        <mylist></mylist>
        <div class="more">
            展开更多文章
            <i class="icon getMore"></i>
        </div>
    </div>
    <mylogin></mylogin>
</div>
</template>
<script>
import header from '@/components/header/header'
import slogan from '@/components/slogan/slogan'
import list from '@/components/list/list'
import type from '@/components/type/type'
import login from '@/components/login/login'
export default {
    components: {
        myheader: header,
        myslogan: slogan,
        mylist: list,
        mytype: type,
        mylogin: login
    }
};
</script>
<style lang="scss" scoped>
.list{
    background: #fff;
    margin-bottom: 0.2rem;
}
.more{
    font-size:0.3rem;
    width: 100%;
    height: 0.8rem;
    line-height: 0.8rem;
    color: #878787;
    text-align: center;
}
.getMore::before{
    content: "\E621";
}
</style>
