<template>
    <section class="hero">
        <div class="nav-bar">
            <img src="../assets/Logo.svg" alt="Logo" class="logo" />
            <img src="../assets/Burger_Menu.svg" alt="Burger" class="burger" />
        </div>
        <div class="hero-content">
            <div class="left-section">
                <h1 class="colored">Scale&nbsp;Fintech</h1>
                <h1>Safe&nbsp;And&nbsp;Secure</h1>
                <p>Ship your fintech products to your customers with fast and reliable processes. Secure and highly customizable. Rise Finance is the best partner for you if you want to scale your finance products worldwide.</p>
                <button>CONSULTATION</button>
            </div>
            <div>
                <img src="../assets/Right Section.svg" alt="Right Section" class="right-section" />
            </div>
        </div>
        <div class="bottom-section">
            <img src="../assets/Logo(2).svg" alt="Bottom Section" class="bottom-section-img" />
            <img src="../assets/Logo(1).svg" alt="Bottom Section" class="bottom-section-img" />
            <img src="../assets/Logo(3).svg" alt="Bottom Section" class="bottom-section-img" />
            <img src="../assets/Logo(4).svg" alt="Bottom Section" class="bottom-section-img" />
        </div>
    </section>
</template>

<script setup></script>

<style scoped>
.hero {
    background: #121139;
    color: white;
    width: 100vw;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}
.nav-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;
    padding: 20px;

}
.hero-content{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;
}

.right-section{
    width: 770px;
}

.left-section{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    width: 695px;
}

h1{
    font-weight: 600;
    font-size: 70px;
    letter-spacing: -4px;
    line-height: 1.1;
    transform: scaleY(1.05);
    transform-origin: center
}
p{
    font-weight: 400;
    font-size: 20px;
    line-height: 130%;
    letter-spacing: 4%;
    margin-top: 20px;
}

h1.colored {
    background: linear-gradient(90deg, #812DE2, #3A49F9);
    color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    display: inline-block;
}

button{
    background: transparent;
    width: 274px;
    height: 74px;
    color: white;
    font-weight: 600;
    font-size: 19px;
    margin-top: 20px;
    border: 0;
    position: relative;
    background-clip: padding-box;
    padding: 4px;
    box-sizing: border-box;
    background: linear-gradient(#121139, #121139) padding-box,
                linear-gradient(90deg, #812DE2, #3A49F9) border-box;
    border: 4px solid transparent;
}
.bottom-section{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 70%;
    margin-bottom: 50px;
}

.bottom-section-img{
    width: 236px;
    height: 51px;
}

</style>

