<template>
    <div class="footer-banner">
        <div class="right-elements">
            <div>
                <h3>DC COMICS</h3>
                <ul>
                    <li v-for="(link, index) in comicsLinks" :key="index" ><a href="#">{{link.text}}</a></li>
                    
                </ul>
                <h3>SHOP</h3>
                <ul>
                    <li v-for="(link, index) in shopLinks" :key="index" ><a href="#">{{link.text}}</a></li>
                    
                </ul>
            </div>
            <div>
                <h3>DC</h3>
                <ul>
                   <li v-for="(link, index) in dcLinks" :key="index" ><a href="#">{{link.text}}</a></li>
                    
                </ul>
            </div>
            <div>
                <h3>SITES</h3>
                <ul>
                    <li v-for="(link, index) in sitesLinks" :key="index" ><a href="#">{{link.text}}</a></li>
                    
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
    data: function() {
        return {
            comicsLinks: [
                {
                    text: 'Charaters',
                },
                {
                    text: 'Comics',
                },
                {
                    text: 'Movies',
                },
                {
                    text: 'TV',
                },
                {
                    text: 'Games',
                },
                {
                    text: 'Videos',
                },
                {
                    text: 'news',
                },
                
            ],
            shopLinks:[
                {
                    text: 'Shop DC'
                },
                {
                    text: 'Shop DC Collectibles'
                },
            ],
            dcLinks:[
                {
                    text:'Terms Of Use'
                },
                {
                    text:'Privacy policy (new)'
                },
                {
                    text:'AD Choices'
                },
                {
                    text:'Advertising'
                },
                {
                    text:'Jobs'
                },
                {
                    text:'Subscription'
                },
                {
                    text:'Talent Workshops'
                },
                {
                    text:'CPSC Certificates'
                },
                {
                    text:'Ratings'
                },
                {
                    text:'Shop Help'
                },
                {
                    text:'Contact Us'
                },
            ],
            sitesLinks:[
                {
                    text:'DC'
                },
                {
                    text:'MAD Magazine'
                },
                {
                    text:'DC Kids'
                },
                {
                    text:'DC Universe'
                },
                {
                    text:'DC Power Visa'
                },
            ],
            
        };
    },
    props: {
    msg: String,
  },
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
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
        width: 40%;
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