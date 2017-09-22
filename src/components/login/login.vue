<template>
    <div class="login">
        <div class="loginBtn">
            <span>登陆</span>
        </div>
        <div class="download">
            <i class="icon download-btn"></i>
            下载简书，创作你的创作
        </div>
    </div>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
.login{
    height: 2rem;
    font-size:0.26rem;
    background: #fff;
    padding-bottom:0.3rem;
    &Btn{
        height:1rem;
        line-height: 1rem;
        text-align: center;
        span{
            display: block;
            width: 1rem;
            height: 1rem;
            margin:0 auto;
            color: #878787;
        }
    }
    .download{
        height:0.95rem;
        background:#e35849;
        width:90%;
        border-radius: 0.1rem;
        line-height:0.95rem;
        text-align: center;
        margin: 0 auto;
        font-size: 0.3rem;
        color: #fff;
        .download-btn::after{
            content: "\E69D"
        }
    }
}
</style>
