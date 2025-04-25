<template>
  <section class="frame">
      <div class="frame-content">
          <div class="frame-text">
              <h1>Consulting For Startups In Fintech</h1>
              <p>Our Team consists of proven experts from finance, tech and science. This mix makes it possible for our team to deliver the best results to all our clients.</p>
          </div>
          <img src="../assets/Component 2.png" alt="Frame 1" />
      </div>
  </section>
</template>

<script setup></script>

<style scoped>
.frame{
  background: #ffffff;
  color:#121139;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 80px;
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
  justify-content: center;
  align-items: center;
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
  line-height: 100%;
}

p{
  font-weight: 500;
  font-size: 22px;
  line-height: 130%;
  letter-spacing: 4%;
  margin-top: 20px;
  width: 510px;
  text-align: center;
}


@media (max-width: 1440px) {
  .frame {
    height: auto;
    min-height: 80vh;
  }
  
  .frame-content {
    max-width: 1200px;
    gap: 30px;
  }
  
  h1 {
    max-width: 650px;
    width: 100%;
  }
  
  p {
    max-width: 500px;
    width: 100%;
  }
}

@media (max-width: 1200px) {
  .frame {
    padding: 40px 20px;
  }
  
  h1 {
    font-size: 45px;
    max-width: 600px;
  }
  
  p {
    font-size: 20px;
    max-width: 450px;
  }
  
  img {
    max-width: 450px;
    height: auto;
  }
}

@media (max-width: 1024px) {
  .frame {
    height: auto;
    min-height: 100vh;
    margin-top: 50px;
    padding: 50px 20px;
  }
  
  .frame-content {
    flex-direction: column;
    align-items: center;
    gap: 40px;
    width: 100%;
  }

  .frame-text {
    align-items: center;
    text-align: center;
    max-width: 600px;
  }

  h1 {
    font-size: 40px;
    letter-spacing: -0.5px;
    width: 100%;
    max-width: 100%;
    transition: all 0.3s ease;
  }

  p {
    font-size: 18px;
    width: 100%;
    max-width: 550px;
    transition: all 0.3s ease;
  }

  img {
    max-width: 400px;
    width: 90%;
    height: auto;
    transition: all 0.3s ease;
  }
}

@media (max-width: 768px) {
  .frame {
    padding: 40px 15px;
    margin-top: 40px;
  }
  
  .frame-content {
    gap: 30px;
  }
  
  h1 {
    font-size: 32px;
    line-height: 1.2;
  }

  p {
    font-size: 16px;
    line-height: 1.5;
    margin-top: 15px;
  }

  img {
    max-width: 350px;
    width: 85%;
  }
}

@media (max-width: 480px) {
  .frame {
    padding: 30px 15px;
    margin-top: 30px;
    min-height: 80vh;
  }
  
  .frame-content {
    gap: 25px;
  }
  
  h1 {
    font-size: 24px;
    line-height: 1.3;
    padding: 0 5px;
  }

  p {
    font-size: 14px;
    line-height: 1.6;
    margin-top: 12px;
    padding: 0 10px;
  }

  img {
    max-width: 280px;
    width: 90%;
  }
}

@media (max-width: 360px) {
  .frame {
    padding: 20px 10px;
  }
  
  h1 {
    font-size: 20px;
  }

  p {
    font-size: 13px;
    margin-top: 10px;
  }

  img {
    max-width: 230px;
  }
}

</style>