<template>
  <section class="frame">
      <div class="frame-content">
          <div class="frame-text">
              <h1>Coruma Finance</h1>
              <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.</p>
          </div>
          <div class="info">
            <div class="txt-box-a"><div class="txt">Accquired 8 long time customers</div></div>
            <div class="txt-box-b"><div class="txt">300% Growth in first year</div></div>
            <div class="txt-box-c"><a class="txt">hired 24 talented developers</a></div>
          </div>
      </div>
  </section>
</template>

<style scoped>
.frame{
    background-image: url("../assets/background.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    background-color: #121139;
  color:#ffffff;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 80px;
}

.frame-content{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  width: 90%;
}

.frame-title{
  display: flex;
  flex-direction: column;
  justify-content: space-between;

  align-items: center;
  width: 100%;
}

.frame-text{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  width: 723px;
  height: 100%;
  margin-bottom: 90px;
}

h1 {
  background: linear-gradient(90deg, #9030F4, #4945F8);
  color: transparent;
  -webkit-background-clip: text;
  background-clip: text;
  display: inline-block;
  width: 724px;
  font-weight: 600;
  font-size: 50px;
  text-align: center;
  line-height: 100%;
}

p{
  font-weight: 500;
  font-size: 22px;
  line-height: 130%;
  letter-spacing: 4%;
  margin-top: 20px;
  width: 911px;
  text-align: center;
}

.info{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  width: 1170px;
  height: 500px;
  background-image: url('../assets/iMac.png');
  background-position: center; /* Centers the image */
  background-repeat: no-repeat;
}

.txt-box-c{
    width: 100%;
    height: 112px;
    display: flex;
    justify-content: flex-end;
}

.txt-box-a {
    width: 100%;
    height: 112px;
    display: flex;
    justify-content: flex-end;
}

.txt-box-b {
    width: 100%;
    height: 112px;
    display: flex;
    justify-content: flex-start;
}
.txt {
    width: 432px;
    height: 118px;
    font-weight: 500;
    font-size: 20px;
    background-color: #1C1A50;
    display: flex;
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
    border-radius: 30px;
    overflow: visible;
}


@media (max-width: 1280px) {
  .frame-text {
    width: 100%;
    max-width: 723px;
  }
  
  h1 {
    width: 100%;
    font-size: 45px;
  }
  
  p {
    width: 100%;
    max-width: 800px;
    font-size: 20px;
  }
  
  .info {
    width: 100%;
    background-size: contain;
    height: 450px;
  }
  
  .txt {
    width: 380px;
  }
}

@media (max-width: 1024px) {
  .frame {
    height: auto;
    min-height: 100vh;
    padding: 60px 0;
  }
  
  .frame-content {
    gap: 40px;
  }
  
  .frame-text {
    margin-bottom: 40px;
  }
  
  h1 {
    font-size: 40px;
  }
  
  p {
    font-size: 18px;
  }
  
  .info {
    height: 400px;
    background-size: 90%;
  }
  
  .txt-box-a, .txt-box-b, .txt-box-c {
    height: 90px;
  }
  
  .txt {
    width: 350px;
    height: auto;
    min-height: 90px;
    font-size: 18px;
    padding: 15px;
  }
}

@media (max-width: 768px) {
  .frame {
    padding: 40px 0;
  }
  
  h1 {
    font-size: 32px;
  }
  
  p {
    font-size: 16px;
  }
  
  .info {
    height: auto;
    background-image: none;
    gap: 20px;
  }
  
  .txt-box-a, .txt-box-b, .txt-box-c {
    width: 100%;
    height: auto;
    display: flex;
    justify-content: center;
  }
  
  .txt {
    width: 90%;
    max-width: 400px;
    font-size: 16px;
    padding: 15px 20px;
    transition: all 0.3s ease;
  }
}

@media (max-width: 480px) {
  .frame {
    padding: 30px 15px;
  }
  
  h1 {
    font-size: 28px;
  }
  
  p {
    font-size: 14px;
    line-height: 1.5;
  }
  
  .txt {
    width: 95%;
    font-size: 14px;
    padding: 12px 15px;
    border-radius: 20px;
    border-width: 1px;
  }
}

@media (max-width: 360px) {
  h1 {
    font-size: 24px;
  }
  
  .txt {
    padding: 10px;
    font-size: 13px;
  }
}

</style>