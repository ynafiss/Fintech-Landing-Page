<template>
    <section class="frame">
        <div class="frame-title">
            <h1>Delivering Value In Every Step Of Production</h1>
        </div>
        <div class="frame-content">
            <img class="chart-box" src="../assets/Circle Chart.png" alt="Frame 2" />
            <div class="frame-text">
                <div>
                    <h2>The Process</h2>
                    <p>Strategic phrases we run through with every client make it possible to implement highly efficinet processes, even in high pace startups that like to scale as fast as possible.</p>
                </div>
                <div class="container">
                    <div
                        v-for="(box, index) in processSteps"
                        :key="index"
                        class="boxes"
                    >
                        <img :src="box.icon" :alt="box.title" style="width: 70px; height: 70px;" />
                        <a style="width: 100%; height: 29px; font-weight: 500; font-size: 22px; line-height: 150%; text-align: center; margin-top: 40px;">
                            {{ box.title }}
                        </a>
                        <div class="number-container">
                            <h1 class="step-number">{{ box.step }}</h1>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>


<script setup lang="ts">
import chartGrowthIcon from "../assets/uil_chart-growth.png";
import arrowGrowthIcon from "../assets/uil_arrow-growth.png";
import moneyIcon from "../assets/fluent_money-20-regular.png";

const processSteps: ProcessStep[] = [
    { title: "Analysis", icon: chartGrowthIcon, step: 1 },
    { title: "Growth Phase", icon: arrowGrowthIcon, step: 2 },
    { title: "Profit", icon: moneyIcon, step: 3 },
];
type ProcessStep = {
    title: string;
    icon: string;
    step: number;
}

</script>

<style scoped>
.frame{
    background-image: url("../assets/bg1.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    background-color: #121139;
    color: white;
    width: 100vw;
    height: 110vh;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 80px;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    overflow: hidden;
}


.frame-title{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
}

.frame-content{
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 90%;
    margin-bottom: 80px;
}

.frame-text{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: space-between;
    width: 723px;
    height: 100%;
}

.container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 100%;
}

.boxes{
    width: 225px;
    height: 192px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border: 0;
    position: relative;
    background-clip: padding-box;
    padding: 4px;
    box-sizing: border-box;
    background: linear-gradient(#1C1A50, #1C1A50) padding-box,
                linear-gradient(90deg, #812DE2, #3A49F9) border-box;
    border: 2px solid transparent;
    border-radius: 40px;
    overflow: visible;
}

h2{
    font-weight: 600;
    font-size: 30px;
    line-height: 100%;
    letter-spacing: -4px;
    margin-bottom: 20px;
}

.number-container {
    position: absolute;
    text-align: center;
    bottom: -85px;
    height: 117px;
}

.step-number {
    background: linear-gradient(90deg, #812DE2, #3A49F9);
    color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    height: 117px;
    width: auto;
    font-size: 90px;
    font-weight: 500;
    line-height: 130%;
    letter-spacing: 4%;
    text-align: center;
}

h1 {
    background: linear-gradient(90deg, #4646F9, #9130F4);
    color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    display: inline-block;
    width: 724px;
    font-weight: 600;
    font-size: 50px;
    text-align: center;
}   
p{
    font-weight: 500;
    font-size: 22px;
    line-height: 130%;
    letter-spacing: 4%;
    line-height: 130%;
    margin-top: 20px;

}

.chart-box{
    border-radius: 10px;
    box-shadow: 0 0 305px #812DE2, 0 0 25px rgba(129, 45, 226, 0.5);
}

@media (max-width: 1440px) {
  .frame {
    height: auto;
    min-height: 100vh;
  }
  
  .chart-box {
    max-width: 90%;
    height: auto;
  }
  
  .frame-text {
    width: 100%;
    max-width: 723px;
  }
  
  h1 {
    width: 100%;
    max-width: 724px;
  }
}

@media (max-width: 1200px) {
  .frame-content {
    width: 95%;
  }
  
  .container {
    gap: 20px;
  }
  
  .boxes {
    width: 200px;
    height: 180px;
  }
  
  .number-container {
    bottom: -70px;
  }
  
  .step-number {
    font-size: 80px;
    height: 100px;
  }
}

@media (max-width: 1024px) {
  .frame {
    padding: 60px 20px;
  }
  
  .frame-content {
    flex-direction: column;
    align-items: center;
    gap: 60px;
    margin-bottom: 40px;
  }

  .frame-text {
    align-items: center;
    text-align: center;
  }
  
  .chart-box {
    max-width: 80%;
    box-shadow: 0 0 150px #812DE2, 0 0 15px rgba(129, 45, 226, 0.5);
  }

  h1 {
    font-size: 40px;
    width: 100%;
  }
  
  h2 {
    font-size: 28px;
    letter-spacing: -2px;
  }

  p {
    font-size: 18px;
  }

  .container {
    justify-content: center;
    gap: 30px;
    margin-top: 40px;
    flex-wrap: wrap;
  }
  
  .boxes {
    width: 200px;
    height: 180px;
    margin-bottom: 90px;
    transition: all 0.3s ease;
  }

  .step-number {
    font-size: 70px;
  }
}

@media (max-width: 768px) {
  .frame {
    padding: 50px 15px;
  }
  
  .chart-box {
    max-width: 90%;
    box-shadow: 0 0 100px #812DE2, 0 0 10px rgba(129, 45, 226, 0.5);
  }
  
  h1 {
    font-size: 32px;
    letter-spacing: -1px;
  }
  
  h2 {
    font-size: 24px;
    letter-spacing: -1px;
  }

  p {
    font-size: 16px;
  }

  .boxes {
    width: 180px;
    height: 160px;
    border-radius: 30px;
    margin-bottom: 80px;
  }

  .step-number {
    font-size: 60px;
    height: 90px;
  }
  
  .number-container {
    bottom: -60px;
  }
  
  img.box-icon {
    width: 60px !important;
    height: 60px !important;
  }
}

@media (max-width: 600px) {
  .frame {
    margin-top: 40px;
  }
  
  .container {
    flex-direction: column;
    gap: 90px;
  }
  
  .boxes {
    width: 220px;
    height: 180px;
    margin-bottom: 0;
  }
  
  .number-container {
    bottom: -50px;
  }
}

@media (max-width: 480px) {
  .frame {
    padding: 40px 10px;
  }
  
  h1 {
    font-size: 24px;
    letter-spacing: -0.5px;
  }
  
  h2 {
    font-size: 20px;
    letter-spacing: normal;
    margin-bottom: 10px;
  }

  p {
    font-size: 14px;
  }

  .boxes {
    width: 200px;
    height: 160px;
    border-radius: 25px;
    border-width: 1px;
  }

  .step-number {
    font-size: 50px;
    height: 70px;
  }
  
  img.box-icon {
    width: 50px !important;
    height: 50px !important;
  }
  
  .chart-box {
    box-shadow: 0 0 70px #812DE2, 0 0 7px rgba(129, 45, 226, 0.5);
  }
}

@media (max-width: 360px) {
  h1 {
    font-size: 20px;
  }
  
  h2 {
    font-size: 18px;
  }
  
  p {
    font-size: 13px;
  }
  
  .boxes {
    width: 180px;
    height: 150px;
  }
  
  img.box-icon {
    width: 45px !important;
    height: 45px !important;
  }
}

</style>