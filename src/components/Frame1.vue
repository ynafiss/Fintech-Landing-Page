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

.frame-text{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
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
    text-align: center;
}

</style>