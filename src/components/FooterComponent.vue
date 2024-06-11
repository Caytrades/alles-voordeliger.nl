<template>
    <footer>
        <div class="content">
            <a href="#">&copy;2023 Your Leads</a>
            <div class="line"></div>
            <a href="#">Actievoorwaarden</a>
            <div class="line"></div>
            <a href="#">Privacy Policy</a>
            <div class="line"></div>
            <a href="#">Over ons</a>
        </div>
    </footer>
</template>


<script>

</script>


<style scoped>
    footer{
        margin-top: 20px ;
        background-color: #160C06;
    }



    .line{
        background-color: #4B4745;
        height: 2px;
        width: 25px;
        transform: rotate(90deg);
        margin-top: 5px;
    }

    .content{
        margin-left: 30px;
        padding: 15px;
        display: flex;
    }

    .content a{
        text-decoration: none;
        color: #4B4745;
        font-weight: 700;
        font-size: 11px;
    }
</style>