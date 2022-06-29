<template>
    <div class="wrapper">
        <header>
            <span class="title">
                PomoFocus
            </span>
        </header>
        <main>
            <div class="circleAndText">
                <!-- Circle-->
                <div class="containerCircle">
                    <div class="circle">
                        
                    </div>
                    <div class="circleText">
                        5:00
                    </div>
                </div>

                <!--Tasks and Grousp-->
                <div class="text">
                    <div class="task">
                        <span>
                            Task
                        </span>
                        <button class="btn">
                            +
                        </button>
                    </div>
                    <div class="group">
                        <span>
                            Group
                        </span>
                        <button class="btn">
                            +
                        </button>
                    </div>
                </div>
            </div>

            <!--Gear SVG-->
            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="#81D8F7" class="bi bi-gear-fill" viewBox="0 0 16 16">
                <path d="M9.405 1.05c-.413-1.4-2.397-1.4-2.81 0l-.1.34a1.464 1.464 0 0 1-2.105.872l-.31-.17c-1.283-.698-2.686.705-1.987 1.987l.169.311c.446.82.023 1.841-.872 2.105l-.34.1c-1.4.413-1.4 2.397 0 2.81l.34.1a1.464 1.464 0 0 1 .872 2.105l-.17.31c-.698 1.283.705 2.686 1.987 1.987l.311-.169a1.464 1.464 0 0 1 2.105.872l.1.34c.413 1.4 2.397 1.4 2.81 0l.1-.34a1.464 1.464 0 0 1 2.105-.872l.31.17c1.283.698 2.686-.705 1.987-1.987l-.169-.311a1.464 1.464 0 0 1 .872-2.105l.34-.1c1.4-.413 1.4-2.397 0-2.81l-.34-.1a1.464 1.464 0 0 1-.872-2.105l.17-.31c.698-1.283-.705-2.686-1.987-1.987l-.311.169a1.464 1.464 0 0 1-2.105-.872l-.1-.34zM8 10.93a2.929 2.929 0 1 1 0-5.86 2.929 2.929 0 0 1 0 5.858z"/>
            </svg>
            <!--Gear SVG-->
        </main>
    </div>

  <RouterView />
</template>

<script setup lang="ts">


</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,500;1,500&family=Roboto:ital,wght@0,400;0,500;0,700;1,700&display=swap');

*{
    margin: 0px;
    padding: 0px;
    font-family: Roboto;
    font-weight: 500;
}

body{
    background-color: #fff;
}

header{
    background-color:#c4c4cc78;
    display: flex;
    align-items: center;
    justify-content: center;
    border-bottom: 5px solid rgba(28,110,164,0.3);
}

.title{
    font-size: 3em;
    font-style: italic;
    font-weight: 500;
    padding: 0.15em;
    color: #000;
}

.circle {
    background-color:#fff;
    border:5px solid red;    
    height:100px;
    border-radius:50%;
    -moz-border-radius:50%;
    -webkit-border-radius:50%;
    width:100px;
}

.circleText{
    display: flex;
    align-items: center;
    justify-content: center;
}

main{
    width: 500px;
    height: 500px;
    display: flex;
    flex-direction:row;
    align-items: center;
    align-content: center;
    justify-content: space-between;
    border: 9px solid #81d8f7;
}

.circleAndText{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.btn{
    border: 2px solid #81d8f7;
    background-color: #fff;
    color: #81d8f7;
    transition: 0.5s;
}

.btn:hover{
    cursor: pointer;
    background-color: rgb(215, 215, 215);
    border: 2px solid #68a8bf;
    transition: 0.5s;
}

SVG{
   fill:#81d8f7;
    transition: 0.5s; 
}

SVG:hover{
    cursor: pointer;
    fill:#68a8bf;
    transition: 0.5s;
}
</style>
