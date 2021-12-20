<template>
    <header>
        <div class="menu-logo">
            <img src="../assets/img/dc-logo.png" alt="logo dc">
        </div>
        <div class="menu">
            <ul>
                <li v-for="(link, index) in links" :key="index" ><a :class="{active: link.active}" href="#"> {{ link.text }}</a></li>
                
            </ul>
        </div>
    </header>
</template>
<script>


export default {
    name: "Header",
    data: function() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    active: false
                },
                {
                    text: 'COMICS',
                    active: true
                },
                {
                    text: 'MOVIES',
                    active: false
                },
                {
                    text: 'TV',
                    active: false
                },
                {
                    text: 'GAMES',
                    active: false
                },
                {
                    text: 'COLLECTIBLES',
                    active: false
                },
                {
                    text: 'VIDEOS',
                    active: false
                },
                {
                    text: 'FANS',
                    active: false
                },
                {
                    text: 'NEWS',
                    active: false
                },
                {
                    text: 'SHOP',
                    active: false
                },
            ]
            
        };
    },
    props: {
    msg: String,
  },
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
header{
    height: 100px;
    width: 100%;
    background-color: white;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    .menu-logo{
        display: inline-block;
        img{
            width: 80px;
            height: auto;
        }
    }
    .menu{
        display: inline-block;
        ul{
            list-style-type: none;
            li{
                display: inline;
                padding: 0 20px;
                
                a{
                    text-decoration: none;
                    color: black;
                    padding: 36px 0;
                    font-size: 12px;
                }
                
            }
            .active{
                color: $primary-color;
                border-bottom:6px solid $primary-color ;
            }
        }
    }
}
</style>
