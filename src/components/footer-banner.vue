<template>
    <div class="footer-banner">
        <div class="right-elements">
            <div>
                <h3>DC COMICS</h3>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                </ul>
                <h3>SHOP</h3>
                <ul>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                </ul>
            </div>
            <div>
                <h3>DC</h3>
                <ul>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa di molto </a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                </ul>
            </div>
            <div>
                <h3>SITES</h3>
                <ul>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                    <li><a href="#">qualcosa</a></li>
                </ul>
            </div>
        </div>
        <div class="left-elements">
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </div>
</template>
<script>


export default {
    name: "footerBanner",
    props: {
    msg: String,
  },
}
</script>

<style lang="scss" scoped>
.footer-banner{
    background-image: url("../assets/img/footer-bg.jpg");
    height: 400px;
    display: flex;
    justify-content: space-around;
    overflow: hidden;
    .left-elements{
        align-self: center;
        
        img{
            height: 500px;
            width: auto;
        }
    }
    .right-elements{
        display: flex;
        justify-content: space-between;
        width: 35%;
        div{
            width: calc(100% / 3);
            padding: 20px;
            text-align: left;
            h3{
                color: white;
                margin: 11px 0 12px 0;
            }
            a{
                color: #546873;
            }
        }
            
            
    }
}


</style>