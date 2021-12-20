<template>
    <header>
        <div class="menu-logo">
            <img src="../assets/img/dc-logo.png" alt="logo dc">
        </div>
        <div class="menu">
            <ul>
                <li><a href="#"> testo</a></li>
                <li><a href="#"> testo</a></li>
                <li><a href="#"> testo</a></li>
                <li><a href="#"> testo</a></li>
                <li><a href="#"> testo</a></li>
                <li><a href="#"> testo</a></li>
                <li><a href="#"> testo</a></li>
                <li><a href="#"> testo</a></li>
                <li><a href="#"> testo</a></li>
                <li ><a class="active" href="#"> testo</a></li>
            </ul>
        </div>
    </header>
</template>
<script>


export default {
    name: "Header",
    props: {
    msg: String,
  },
}
</script>

<style lang="scss" scoped>
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
                    padding: 35px 0;
                }
                
            }
            .active{
                color: #0c7cec;
                border-bottom:6px solid #0c7cec ;
            }
        }
    }
}
</style>
