<template>
    <section class="frame">
        <div class="frame-title">
            <h1>Case Study</h1>
            <p>Some results from our clients</p>
        </div>
        <div class="frame-content">
            <div class="left-section">
                <div class="left-section-text">
                    <h2>Coruma Finance</h2>
                    <p style="width: 480px;">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.</p>
                    <button>READ MORE ABOUT THIS CLIENT</button>
                </div>
                <img class="logo" src="../assets/Logo.png" alt="logo" />
            </div>
            <div class="right-section">
                <img style="z-index: 100;" src="../assets/Phone.png"  alt="Frame 3" />
                <div class="frame-text">
                    <a>Accquired 8 long time customers</a>
                    <a>300% Growth in first year</a>
                    <a>hired 24 talented developers</a>
                </div>
            </div>
        </div>
    </section>

</template>

<style scoped>
.frame{
    background: #ffffff;
    color: #121139;
    width: 100vw;
    height: 150vh;
    display: flex;
    justify-content: center;
    align-items: center;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    overflow: hidden;
}

.frame-title{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    width: 100%;
}

.frame-content{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 90%;
}

.right-section{
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 919px;
    background-color: transparent;
}

.left-section{
    background-image: url("../assets/background.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    background-color: #121139;
    width: 919px;
    height: 919px;
    margin-right: -200px;
    overflow: visible;
    display: flex;
    align-items: center;
    border-radius: 30px;
}
.left-section-text{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    color: #ffffff;
    width: 480px;
    margin-left: 50px;
}

.frame-text{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: space-between;
    width: 723px;
    height: 100%;
}

a{
    height: 112px;
    width: 486px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: 500;
    font-size: 20px;
    line-height: 130%;
    letter-spacing: 4%;
    margin-top: 20px;
    margin-bottom: 40px;
    margin-left: -38px;
    color: #ffffff;
    border: 0;
    position: relative;
    background-clip: padding-box;
    padding: 4px;
    box-sizing: border-box;
    background: linear-gradient(#1C1A50, #1C1A50) padding-box,
                linear-gradient(90deg, #812DE2, #3A49F9) border-box;
    border: 2px solid transparent;
    border-radius: 20px;
}

h1{
    background: linear-gradient(90deg, #812DE2, #3A49F9);
    color: transparent;
    -webkit-background-clip: text;
    background-clip: text;
    font-weight: 600;
    font-size: 50px;
    letter-spacing: 0px;
    line-height: 100%;
    transform: scaleY(1.05);
    transform-origin: center;
    margin-bottom: 30px;
}

p{
    font-weight: 500;
    font-size: 22px;
    line-height: 130%;
    letter-spacing: 1px;
    margin-top: 20px;
    margin-bottom: 10px;
}

h2{
    font-weight: 600;
    font-size: 30px;
    line-height: 100%;
    margin-bottom: 50px;
}

button{
    background: transparent;
    width: 411px;
    height: 74px;
    color: white;
    font-weight: 600;
    font-size: 19px;
    margin-top: 50px;
    border: 0;
    position: relative;
    background-clip: padding-box;
    padding: 4px;
    box-sizing: border-box;
    background: linear-gradient(#121139, #121139) padding-box,
                linear-gradient(90deg, #812DE2, #3A49F9) border-box;
    border: 4px solid transparent;
}


@media (max-width: 1440px) {
  .frame {
    height: auto;
    min-height: 100vh;
    padding: 60px 0;
  }
  
  .left-section {
    margin-right: -100px; 
  }
}

@media (max-width: 1200px) {
  .frame {
    padding: 50px 0;
  }
  
  .left-section {
    width: 60%;
    margin-right: -80px;
  }
  
  .right-section {
    width: 60%;
  }
  
  .left-section-text {
    width: 90%;
    max-width: 450px;
  }
  
  a {
    width: 90%;
    max-width: 400px;
    margin-left: 0;
  }
  
  .logo {
    max-width: 150px;
    position: absolute;
    bottom: 30px;
    right: 30px;
  }
}

@media (max-width: 1024px) {
  .frame {
    padding: 40px 20px;
  }
  
  .frame-content {
    flex-direction: column;
    align-items: center;
    gap: 40px;
  }
  
  .left-section {
    width: 95%;
    max-width: 800px;
    height: auto;
    min-height: 500px;
    margin-right: 0;
    padding: 40px 0;
    position: relative;
  }
  
  .left-section-text {
    align-items: center;
    text-align: center;
    margin-left: 0;
    width: 90%;
    max-width: 600px;
    padding: 0 20px;
  }
  
  .left-section-text p {
    width: 100% !important; 
  }
  
  .right-section {
    width: 95%;
    max-width: 800px;
    flex-direction: column;
    justify-content: center;
    gap: 30px;
  }
  
  .right-section img {
    max-width: 80%;
    height: auto;
  }
  
  .frame-text {
    width: 100%;
    align-items: center;
  }
  
  a {
    width: 90%;
    max-width: 500px;
    font-size: 18px;
    margin-bottom: 20px;
    transition: all 0.3s ease;
  }
  
  button {
    width: 80%;
    max-width: 400px;
    font-size: 16px;
  }
}

@media (max-width: 768px) {
  .frame {
    padding: 30px 15px;
  }
  
  h1 {
    font-size: 40px;
  }
  
  h2 {
    font-size: 24px;
    margin-bottom: 30px;
  }
  
  p {
    font-size: 18px;
  }
  
  .left-section {
    min-height: 400px;
  }
  
  a {
    font-size: 16px;
    height: auto;
    padding: 15px;
    border-width: 2px;
  }
  
  button {
    height: 60px;
    border-width: 3px;
  }
  
  .logo {
    max-width: 120px;
    bottom: 20px;
    right: 20px;
  }
}

@media (max-width: 480px) {
  .frame {
    padding: 25px 10px;
  }
  
  .frame-title {
    margin-bottom: 20px;
  }
  
  h1 {
    font-size: 32px;
  }
  
  h2 {
    font-size: 20px;
    margin-bottom: 20px;
  }
  
  p {
    font-size: 16px;
  }
  
  .left-section {
    min-height: 350px;
    border-radius: 20px;
  }
  
  a {
    font-size: 14px;
    padding: 12px;
    border-radius: 15px;
    margin-bottom: 15px;
  }
  
  button {
    font-size: 14px;
    height: 50px;
    margin-top: 30px;
  }
  
  .logo {
    max-width: 100px;
    bottom: 15px;
    right: 15px;
  }
}

@media (max-width: 360px) {
  h1 {
    font-size: 28px;
  }
  
  h2 {
    font-size: 18px;
  }
  
  p {
    font-size: 14px;
  }
  
  a {
    font-size: 13px;
    padding: 10px;
  }
  
  button {
    font-size: 12px;
    height: 45px;
  }
}
</style>