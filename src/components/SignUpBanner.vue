<script>
export default{
    methods: {
        register() {
            this.$router.push('/success')
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
                <form class="input-field">
                        <input type="text" placeholder="Voonaam" required>
                        <input type="text" placeholder="Achternaam" required>
                        <input type="text" placeholder="Telefoonnummer" required>
                        <button @click="register" type="submit">Volgende stap</button>
                </form>
                <div class="line"></div>
                <p style="color: white; font-size: 15px;">Dit wordt mogelijk gemaakt door Alles Voordeliger.nl</p>
            </div>
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
    font-family: fantasy;
    font-size: 100px;
    margin: unset;
    transform: rotate(-10deg);
    margin-left: 50px;
    font-weight: 900;
}

.first h4{
    font-size: 60px;
    font-family: fantasy;
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


    
</style>