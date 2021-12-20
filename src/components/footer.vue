<template>
    <footer>
        <div class="btn">
            <a href="#">SIGN-UP NOW!</a>
        </div>
        <div class="social-media-link">
            <span>FOLLOW US</span>
            <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
            <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
            <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
            <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
            <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
        </div>
    </footer>
</template>
<script>


export default {
    name: "Footer",
    props: {
    msg: String,
  },
}
</script>
<style lang="scss" scoped>
@import '../style/variables';
footer{
    height: 100px;
    width: 100%;
    background-color: #303030;
    display: flex;
    justify-content: space-around;
    align-items: center;
    .btn{
        padding: 4px 10px;
        border: 2px solid $primary-color;
        a{
            color: white;
        }
        
    }
    .social-media-link{
        span{
            vertical-align: super;
        }
        a{
            padding: 10px;
        }
    }
}
</style>