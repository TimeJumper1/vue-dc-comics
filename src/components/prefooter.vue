<template>
    <main>
        <div class="container">
            <ul>
                <li><a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt="">DIGITAL COMICS</a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-merchandise.png" alt="">DC MERCHANDISE</a></li>
                <li><a href="#"><img src="../assets/img/buy-comics-subscriptions.png" alt="">SUBSCRIPTION</a></li>
                <li><a href="#"><img class="smaller" src="../assets/img/buy-comics-shop-locator.png" alt="">COMIC SHOP LOCATOR</a></li>
                <li><a href="#"><img src="../assets/img/buy-dc-power-visa.svg" alt="">DC POWER VISA</a></li>
            </ul>
        </div>
    </main>
</template>
<script>


export default {
    name: "prefooter",
    props: {
    msg: String,
  },
}
</script>

<style lang="scss" scoped>

main{
    height: 130px;
    width: 100%;
    background-color: #0c7cec;
    color: white;
    .container{
        height: 100%;
        ul{
            list-style-type: none;
            display: flex;
            flex-direction: row;
            width: 100%;
            justify-content: space-evenly;
            align-items: center;
            line-height: 130px;
            li{
                

                
                
                a{
                    text-decoration: none;
                    color:inherit ;
                    display: flex;
                    align-items: center;
                    img{
                        width: 55px;
                        height: auto;
                    }
                    .smaller{
                        width: 40px;
                        height: auto;
                    }
                }
                
            }
            
        }
        
    }
}


</style>