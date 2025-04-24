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
                <div>
                    <div class="boxes">
                        <img src="../assets/uil_chart-growth.png" style="width: 70px;height: 70px;" alt="Frame 2" />
                        <a style="width: 99px; height: 29px; font-weight: 500; font-size: 22px; line-height: 150%;" >Analysis</a>
                        <div class="number-container">
                            <h1 class="step-number">1</h1>
                        </div>>
                    </div>
                    <div></div>
                    <div></div>
                </div>
            </div>
        </div>
    </section>

</template>

<script setup></script> 

<style scoped>
.frame{
    background: #121139;
    color: white;
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 80px;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
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
}

.frame-text{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: space-between;
    width: 823px;
    height: 100%;
}

.boxes{
    width: 202px;
    height: 172px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border: 0;
    position: relative;
    background-clip: padding-box;
    padding: 4px;
    box-sizing: border-box;
    background: linear-gradient(#121139, #121139) padding-box,
                linear-gradient(90deg, #812DE2, #3A49F9) border-box;
    border: 4px solid transparent;
    overflow: visible;
}

.number-container {
    position: absolute;
    /* right: -20px; */
    bottom: -70px;
    height: 117px;
}

.step-number {
    background: linear-gradient(90deg, #812DE2, #3A49F9);
    color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    height: 117px;
    width: auto;
    font-size: 100px;
    font-weight: 700;
    line-height: 1;
    text-align: center;
}

h1 {
    background: linear-gradient(90deg, #812DE2, #3A49F9);
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
    font-weight: 400;
    font-size: 20px;
    line-height: 130%;
    letter-spacing: 4%;
    margin-top: 20px;
    width: 510px;
}

.chart-box{
    /* border: #812DE2 2px solid; */
    border-radius: 10px;
    box-shadow: 0 0 305px #812DE2, 0 0 25px rgba(129, 45, 226, 0.5);
}

</style>