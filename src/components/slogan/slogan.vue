<template>
    <div class="slogan">
        <ul class="sloganUl">
            <li class="sloganUlLi">随时随地发现和创作内容</li>
            <li class="sloganUlLi">每天为你精选好文</li>
            <li class="sloganUlLi">第一时间收到作者文章更新</li>
        </ul>
        <div class="sloganPhone">
            <img src="static/images/phone.png" alt="">
        </div>
    </div>
</template>
<script>
export default {
    name: "solgan"
};
</script>
<style lang="scss" scoped>
.slogan{
    position: relative;
    width: 100%;
    height: 2.05rem;
    margin-bottom: 0.2rem;
    padding-top: 0.35rem;
    font-size:0.26rem;
    background: #fff;
    &Ul{
        position: relative;
        left:0.7rem;
        height: 1.7rem;
        &Li{
            height: 0.6rem;
            line-height:0.6rem;
            list-style-type: disc;
        }
    }
    &Phone{
        position: absolute;
        top:-0.9rem;
        right:0;
        z-index:1;
        img{
            width:2.2rem;
            height:3.3rem;
        }
    }
}
</style>
