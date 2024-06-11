<script setup>
import {ref} from 'vue'

let isFirst = ref(false)
let isSecond = ref(false)
let isThird = ref(false)
let isFourth = ref(false)
let isFifth = ref(false)

let data = "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam blandit risus eu metus interdum auctor. Morbi molestie pulvinar ullamcorper. Mauris ac auctor nulla, at dignissim felis. Duis rhoncus, justo sit amet elementum eleifend, tortor est efficitur mi, consequat efficitur justo nulla non justo."

</script>

<template >
    <div class="container">
        <div class="faq">
            <div class="line"></div>
            <div class="content">
                <h3>HOE WERKT MET</h3>
                <button @click="isFirst = !isFirst" >+</button>
            </div>
            <p v-show="isFirst">{{data}} </p>
            <div class="line"></div>
            <div class="content">
                <h3>PRIJSUITREIKING</h3>
                <button @click="isSecond = !isSecond" >+</button>

            </div>
            <p v-show="isSecond">{{data}}</p>
            <div class="line"></div>
            <div class="content">
                <h3>ALLES-VOORDELIGER.NL</h3>
                <button @click="isThird = !isThird" >+</button>

            </div>
            <p v-show="isThird">{{data}}</p>
            <div class="line"></div>
            <div class="content">
                <h3>DE VOORWAARDEN</h3>
                <button @click="isFourth = !isFourth" >+</button>

            </div>
            <p v-show="isFourth">{{data}}</p>
            <div class="line"></div>
            <div class="content">
                <h3>DE ORGANISATION</h3>
                <button @click="isFifth = !isFifth" >+</button>

            </div>
            <p v-show="isFifth">{{data}}</p>
            <div class="line"></div>
        </div>
    </div>

    <div class="logo">
        <img src="./img/logo-white.jpg" alt="">
    </div>
</template>


<style scoped>
.container{
    margin-top: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 100px;
}

.faq{
    display: flex;
    flex-direction: column;
    margin-top: 20px;
    max-width: 600px;
}

.line{
    background-color: #000;
    height: 5px;
    width: 600px;
}

.content{
    display: flex;
    justify-content: space-between;
}

.content h3{
    font-weight: 700;
    font-family: fantasy;
}


.content button{
    background: none;
    border: none;
    font-size: 40px;
    font-weight: 700;
}

.logo{
    display: flex;
    justify-content: center;
}

@media only screen and (max-width: 932px) {
    
    .container{
       display: unset;
    }

    .line{
     width: 100%;
    }

    
    
}

@media only screen and (min-width: 768px) {
    .container{
        display: flex;
    }

    .line{
     width: 600px;
    }

}

    
</style>