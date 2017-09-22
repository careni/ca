<template>
    <div class="type">
        <div class="typeHot">
            <h1 class="typeHotTitle">热门专题</h1>
            <span class="typeHotChange" @click="change">
                <i class="icon change" :class="{rotate: rotate}"></i>
                换一批
            </span>
        </div>
        <div class="typeTags">
            <span>连载小说</span>
            <span>历史</span>
            <span>娱乐八卦</span>
            <span>行业故事会</span>
            <span>社会热点</span>
            <span>谈写作</span>
            <span>世间事</span>
        </div>
    </div>
</template>
<script>
export default {
    data () {
        return {
            rotate: false
        };
    },
    created () {},
    methods: {
        change () {
            this.rotate = true;
            // alert(1);
        }
    }
}
</script>
<style lang="scss" scoped>
.type{
    position: relative;
    width: 100%;
    height: 2.5rem;
    background: #fff;
    font-size: 0.26rem;
    margin-bottom: 0.2rem;
    &Hot{
        width:100%;
        height: 0.8rem;
        display: flex;
        justify-content: space-between;
        span,h1{
            display: block;
            height: 0.8rem;
            line-height:0.8rem;
            margin: 0 0.35rem;
        }
        &Title{
            font-size:0.26rem;
        }
        &Change{
            color: #757575;
        }
        .change::before{
            content: "\E6E3"
        }
    }
    &Tags{
        width: 100%;
        display: flex;
        justify-content:flex-start;
        flex-wrap: wrap;
        span{
            padding:0.1rem 0.17rem;
            border:1px solid #e35849;
            color: #e35849;
            border-radius:0.1rem;
            margin-left:0.3rem;
            margin-bottom: 0.22rem;
        }
    }
    @keyframes rolling {
        0%{
            transform: rotate(0deg);
        }
        100%{
            transform: rotate(180deg);
        }
    }
    .rotate::before{
        animation: rolling 0.5s linear;
    }
}
</style>


