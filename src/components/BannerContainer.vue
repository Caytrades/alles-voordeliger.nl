<script>
export default{
    methods: {
        SignUp() {
            this.$router.push('/signup')
        }
    },
}
</script>

<template>
    <div class="banner-container">
        <img src="./img/banner.jpg" alt="">

        <div class="content">
            <div class="logo">
                <img src="./img/banner-logo.jpg" alt="">
            </div>
            <div class="first">
                <h1>Win</h1>
                <h2>€500</h2>
                <h3>Cash</h3>
                <br>
                <h4>DOE MEE EN WIN!</h4>
                <div class="check">
                    <i class="fa-regular fa-circle-check"></i>
                    <strong>Je wint altjid</strong>
                </div>
                <div class="check">
                    <i class="fa-regular fa-circle-check"></i>
                    <p>Geen verplichtinge</p>
                </div>
                <div class="check">
                    <i class="fa-regular fa-circle-check"></i>
                    <p>Een deelname per person</p>
                </div>
                <div class="check">
                    <i class="fa-regular fa-circle-check"></i>
                    <p>Meedoen in 1 minuut</p>
                </div>
                    <form class="input-field">
                        <input type="text" placeholder="E-mailadres" required>
                        <button @click="SignUp" type="submit">DOE MEE!</button>
                    </form>
                <div class="line"></div>
                <p style="color: white; font-size: 15px;">Dit wordt mogelijk gemaakt door Alles Voordeliger.nl</p>
            </div>
        </div>
        <div class="mobile">
            <div class="doe">
                <div class="logo">
                    <img src="./img/banner-logo.jpg" alt="">
                </div>
                <h4>DOE MEE <br> EN WIN!</h4>
            </div>
        </div>
    </div>

    <div class="mobile">
        <div class="container">
            <h3>Maak kans op €500 cashback voor je energiecontracr!</h3>
            <div class="check">
                <i class="fa-regular fa-circle-check"></i>
                <strong>Je wint altjid</strong>
            </div>
            <div class="check">
                <i class="fa-regular fa-circle-check"></i>
                <p>Geen verplichtinge</p>
            </div>
            <div class="check">
                <i class="fa-regular fa-circle-check"></i>
                <p>Een deelname per person</p>
            </div>
            <div class="check">
                <i class="fa-regular fa-circle-check"></i>
                <p>Meedoen in 1 minuut</p>
            </div>
                <form class="input-field">
                    <input type="text" placeholder="E-mailadres" required>
                    <button @click="SignUp" type="submit">DOE MEE!</button>
                </form>
            <div class="line"></div>
            <p style="color: white; font-size: 15px;">Dit wordt mogelijk gemaakt door Alles Voordeliger.nl</p>
        </div>
    </div>
</template>



<style scoped>

.banner-container{
    position: relative;
}

.content{
   position: absolute;
   display: flex;
   gap: 60px;
   top: 2px;
}

.first{
    margin-top: 80px;
}

.first h1,h3{
    font-size: 40px;
    padding: 10px;
    margin: unset;
}


.first h3{
    text-align: end;
}

.first h2{
    font-family: fantasy !important;
    font-size: 100px;
    margin: unset;
    transform: rotate(-10deg);
    margin-left: 50px;
    font-weight: 900;
}

.first h4{
    font-size: 60px;
    font-family: fantasy !important;
    font-weight: 900;
    margin: unset;
}

.logo{
    padding: 10px;
    max-width: 200px;
}

.logo img{
    width: 100%;
}

.logo h2{
    margin: unset;

}

.banner-container img{
    width: 100%;
    border-radius: 10px;
}


.check{
    display: flex;
    gap: 10px;
    margin-bottom: 10px;
}

.check i{
    width: 20px;
}

.check p{
    margin: unset;
}

.input-field{
    display: flex;
    flex-direction: column;
    gap: 20px;
    margin-bottom: 20px;
}

.input-field input{
    background-color: rgba(255, 255, 255, 0);
    padding: 15px;
    border: solid black 2px;
    font-size: 15px;
    font-weight: 600;
    color: rgba(0, 0, 0, 0.377);
}

.input-field button{
    background-color: #060807;
    border: solid white 2px;
    padding: 10px;
    color: white;
    font-size: 20px;
    font-weight: 900;
}

.line{
    background-color: white;
    height: 2px;
}


.mobile{
    display: none;
}

@media only screen and (max-width: 932px) {
    
    .content{
        display: none;
    }

    .mobile{
        display: contents;
    }

    .doe{
        position: absolute;
        display: flex;
        flex-direction: column;
        gap: 10px;
        top: 2px;
    }

    .doe h4{
        font-size: 40px;
        font-family: fantasy !important;
        font-weight: 900;
        margin: unset;
        transform: rotate(-23deg);
        margin-left: 50px;
    }

    .logo{
        padding: unset;
    }

    .logo img{
        width: 50%;
    }

    .container{
        margin-top: 30px; 
       margin-left: 20px;
    }

    .container h3{
        font-size: 20px;
        font-weight: 900;
        font-family: fantasy !important;
    }

    .input-field input{
        width: 300px;
    }

    .input-field button{
        width: 340px;
        background-color: #F2C075 ;
    }
    
}

@media only screen and (min-width: 768px) {

    .content{
        display: flex;
        margin-top: unset;
    }
}

    
</style>