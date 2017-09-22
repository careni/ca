<template>
    <header>
        <div class="logo">
            <img src="static/images/jianshu.png" alt="">
        </div>
        <div class="slogan">创作你的创作</div>
        <div class="download iconfont">
            免费下载
            <i class="icon download-link"></i>
        </div>
    </header>
</template>
<script>
export default {

};
</script>
<style lang="scss" scoped>
$color: #e35849;
header{
    position: fixed;
    top:0;
    width:100%;
    height: 0.96rem;
    background: #fff;
    box-shadow: 0 0 10px 2px #dfdfdf;
    z-index:9999;
    .logo{
        position: absolute;
        left:0.3rem;
        top:0;
        img{
            position: absolute;
            left:0;
            top:0.1rem;
            width:1rem;
            height:0.7rem;
        }
    }
    .slogan{
        position: absolute;
        left:1.5rem;
        top:0;
        height: 0.96rem;
        line-height: 0.96rem;
        font-size:0.3rem;
    }
    .download{
        font-size: 0.3rem;
        color: $color;
        line-height:0.9rem;
        height: 0.9rem;
        position: absolute;
        right: 0;
        top:0;
        .download-link::before{
            content:"\E616";
            position: relative;
            left:-0.1rem;
        }
    }
}
</style>
