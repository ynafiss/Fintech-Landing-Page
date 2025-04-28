<template>
    <section class="hero">
        <div class="nav-bar">
            <img :src="logo" alt="Logo" class="logo" />
            <img :src="burgerMenu" alt="Burger" class="burger" />
        </div>
        <div class="hero-content">
            <div class="left-section">
                <h1 class="colored">Scale&nbsp;Fintech</h1>
                <h1>Safe&nbsp;And&nbsp;Secure</h1>
                <p>Ship your fintech products to your customers with fast and reliable processes. Secure and highly customizable. Rise Finance is the best partner for you if you want to scale your finance products worldwide.</p>
                <button>CONSULTATION</button>
            </div>
            <div>
                <img :src="rightSection" alt="Right Section" class="right-section" />
            </div>
        </div>
        <div class="bottom-section">
            <img
                v-for="(image, index) in bottomSectionImages"
                :key="index"
                :src="image.src"
                :alt="image.alt"
                class="bottom-section-img"
            />
        </div>
    </section>
</template>

<script setup>
import logo from "../assets/Logo.svg";
import burgerMenu from "../assets/Burger_Menu.svg";
import rightSection from "../assets/Right Section.svg";
import bottomSection1 from "../assets/Logo(2).svg";
import bottomSection2 from "../assets/Logo(1).svg";
import bottomSection3 from "../assets/Logo(3).svg";
import bottomSection4 from "../assets/Logo(4).svg";


const bottomSectionImages = [
    { src: bottomSection1 , alt: "Bottom Section 1" },
    { src: bottomSection2 , alt: "Bottom Section 2" },
    { src: bottomSection3 , alt: "Bottom Section 3" },
    { src: bottomSection4 , alt: "Bottom Section 4" }

];
</script>

<style scoped>
.hero {
    background-image: url("../assets/bg1.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    background-color: #121139;
    color: white;
    width: 100vw;
    height: 110vh;
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
    padding-top: 20px;
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
    font-size: 99px;
    letter-spacing: -4px;
    line-height: 1.1;
    text-align: left;
    margin-left: -5px;
}

h1.colored {
  background: linear-gradient(90deg,#4646F9, #9130F4);
    color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
}
p{
    font-weight: 500;
    font-size: 22px;
    line-height: 130%;
    letter-spacing: 4%;
    margin-top: 20px;
    margin-bottom: 10px;
}

button{
    background: transparent;
    width: 274px;
    height: 74px;
    color: white;
    font-weight: 600;
    font-size: 19px;
    margin-top: 30px;
    border: 0;
    position: relative;
    background-clip: padding-box;
    padding: 4px;
    box-sizing: border-box;
    background: linear-gradient(#1c1a52, #1c1a52) padding-box,
                linear-gradient(90deg, #812DE2, #3A49F9) border-box;
    border: 4px solid transparent;
}
.bottom-section{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 70%;
    margin-bottom: 80px;
}


@media (max-width: 1440px) {
  .hero {
    height: auto;
    min-height: 100vh;
  }
  
  .left-section {
    width: 600px;
  }
  
  h1 {
    font-size: 85px;
  }
  
  .right-section {
    width: 650px;
  }
}

@media (max-width: 1200px) {
  .hero-content {
    gap: 30px;
  }
  
  .left-section {
    width: 500px;
  }
  
  h1 {
    font-size: 75px;
    letter-spacing: -3px;
  }
  
  p {
    font-size: 20px;
  }
  
  .right-section {
    width: 550px;
  }
  
  .bottom-section {
    width: 85%;
  }
  
  .bottom-section-img {
    width: 200px;
  }
}

@media (max-width: 1024px) {
  .hero {
    padding: 30px 0;
    justify-content: space-around;
  }
  
  .hero-content {
    flex-direction: column;
    align-items: center;
    gap: 40px;
  }
  
  .left-section {
    width: 90%;
    max-width: 600px;
    align-items: center;
  }
  
  .left-section h1 {
    font-size: 70px;
    text-align: center;
    transition: all 0.3s ease;
  }
  
  .left-section p {
    text-align: center;
    max-width: 550px;
    transition: all 0.3s ease;
  }
  
  .right-section {
    width: 90%;
    max-width: 600px;
    height: auto;
    transition: all 0.3s ease;
  }
  
  button {
    transition: all 0.3s ease;
  }
  
  .bottom-section {
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
  }
}

@media (max-width: 768px) {
  .hero {
    background-position: 75% center;
  }
  
  .nav-bar {
    flex-direction: row;
    gap: 20px;
    padding: 15px;
  }
  
  .logo {
    height: 35px;
  }
  
  .burger {
    height: 25px;
  }
  
  .left-section h1 {
    font-size: 50px;
    letter-spacing: -2px;
  }
  
  .left-section p {
    font-size: 18px;
    padding: 0 20px;
  }
  
  button {
    width: 200px;
    height: 60px;
    font-size: 16px;
    border-width: 3px;
  }
  
  .bottom-section {
    width: 95%;
    margin-bottom: 50px;
    gap: 20px;
  }
  
  .bottom-section-img {
    width: 160px;
    height: auto;
  }
}

@media (max-width: 480px) {
  .hero {
    padding: 20px 0;
  }
  
  .nav-bar {
    width: 95%;
    padding: 10px 0;
  }
  
  .logo {
    height: 30px;
  }
  
  .left-section {
    width: 95%;
  }
  
  .left-section h1 {
    font-size: 40px;
    letter-spacing: -1px;
    line-height: 1.2;
  }
  
  .left-section p {
    font-size: 16px;
    padding: 0 10px;
    line-height: 1.4;
  }
  
  button {
    width: 170px;
    height: 50px;
    font-size: 14px;
    border-width: 3px;
    margin-top: 20px;
  }
  
  .bottom-section {
    margin-bottom: 30px;
  }
  
  .bottom-section-img {
    width: 130px;
  }
}

@media (max-width: 360px) {
  .left-section h1 {
    font-size: 32px;
  }
  
  .left-section p {
    font-size: 14px;
  }
  
  button {
    width: 150px;
    height: 45px;
    font-size: 12px;
    border-width: 2px;
  }
  
  .bottom-section-img {
    width: 110px;
  }
  
  .bottom-section {
    gap: 15px;
  }
}

</style>

