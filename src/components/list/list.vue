<template>
    <div class="list">
        <div class="listUser">
            <img src="static/images/user.jpg" alt="">
            <span>米娜</span>
        </div>
        <div class="listImg" v-if="show" alue="1"></div>
        <div class="listTitle">
            <h1>再白点高点瘦点，我就是别人的老婆了</h1>
        </div>
        <div class="listDescription">亲爱的，山水初相逢，你曾欣喜我如你生命中的一汪清泉，明见你生命中的斑驳阴影。 2017年9月19日  星期二   ...</div>
        <div class="listInfo">
            <span class="tag">世家事</span>
            <span class="info">167评论·888喜欢·999赞赏</span>
        </div>
    </div>
</template>
<script>
export default {
    created () {
        this.$nextTick(() => {
            var a = document.querySelectorAll('.listImg')
            for(var i = 0; i < a.length; i++){
                if(a[i].getAttribute('alue') == "1"){
                    a[i].style.backgroundImage= "url(../../../static/images/demo.jpg)";
                }
            }
        })
    },
    data () {
        return {
            show: false
        }
    }
}
</script>
<style lang="scss" scoped>
.list{
    display: flex;
    flex-direction: column;
    font-size:0.26rem;
    max-height: 7rem;
    width:100%;
    border-bottom: 1px solid #ececec;
    &User{
        width:100%;
        height:1.38rem;
        display:flex;
        >img{
            width:0.68rem;
            height: 0.68rem;
            border-radius:50%;
            border: 1px solid #ececec;
            margin-left:0.35rem;
            margin-top:0.35rem;
        }
        >span{
            position: relative;
            left:0.2rem;
            top:0.55rem;
            font-size: 0.28rem;
        }
    }
    &Img{
        margin:0 0.35rem;
        height: 2.4rem;
        background: no-repeat;
        background-size: cover;
        margin-bottom:0.2rem;
    }
    &Title{
        height:1.1rem;
        padding-right:0.35rem;
        padding-left:0.35rem;
        margin-bottom:0.2rem;
        // font-size:0.36rem;
        >h1{
            height:1.1rem;
            margin:0;
            font-size:0.42rem;
            font-weight: 400;
        }
    }
    &Description{
        padding-right:0.35rem;
        padding-left:0.35rem;
        font-size:0.26rem;
    }
    &Info{
        display: flex;
        justify-content: space-between;
        width:100%;
        margin:0.2rem 0;
        .tag{
            height: 0.26rem;
            line-height: 0.26rem;
            padding:0.07rem 0.12rem;
            border:1px solid #e35849;
            color: #e35849;
            border-radius:0.1rem;
            margin-left:0.35rem;
        }
        .info{
            margin-right:0.35rem;
            color:#878787;
        }
    }
}
</style>

