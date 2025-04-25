<template>
    <section class="frame">
        <div class="frame-header">
            <img src="../assets/Logo_colored.png" alt="Logo"/>
        </div>
        <div class="frame-content">
            <div class="services">
                <h1>Services</h1>
                <ul>
                    <li v-for="(service, index) in services" :key="index">{{ service }}</li>
                </ul>
            </div>
            <div class="support">
                <h1>Support</h1>
                <ul>
                    <li v-for="(item, index) in support" :key="index">{{ item }}</li>
                </ul>
            </div>
            <div class="company">
                <h1>Company</h1>
                <ul>
                    <li v-for="(item, index) in company" :key="index">{{ item }}</li>
                </ul>
            </div>
            <div class="legal">
                <h1>Legal</h1>
                <ul>
                    <li v-for="(item, index) in legal" :key="index">{{ item }}</li>
                </ul>
            </div>
            <div class="subcribe">
                <h1>Subscribe to our newsletter</h1>
                <p>Funding freemium long tail hypotheses first mover advantage assets ownership</p>
            </div>
        </div>
    </section>
</template>


<script setup lang="ts">

interface SectionItem {
    services: string[];
    support: string[];
    company: string[];
    legal: string[];
}

const services: string[] = [
    "Web Hosting",
    "Domains",
    "Premium Hosting",
    "Private Server",
    "E-mail Hosting"
];

const support: string[] = [
    "Pricing Plan",
    "Documentation",
    "Guide",
    "Tutorial"
];

const company: string[] = [
    "About",
    "Blog",
    "Join Us",
    "Press",
    "Partners"
];

const legal: string[] = [
    "Claim",
    "Privacy",
    "Terms"
];
</script>

<style scoped>
.frame{
    background: #121139;
    color: white;
    width: 100vw;
    height: 50vh;
    display: flex;
    justify-content: center;
    align-items: center;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

.frame-header{
    display: flex;
    justify-content: flex-start;
    align-items: center;
    width: 80%;
}
.frame-content{
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    width: 80%;
}

ul{
    list-style: none;
    padding: 0;
    margin-bottom: 20px;
}

h1{
    margin-bottom: 20px;
    color: #92989F;
    font-weight: 600;
    font-size: 18px;
}

li{

    color: #ffffff;
    font-weight: 400;
    font-size: 16px;
    margin-bottom: 10px;
}

@media (max-width: 1200px) {
    .frame {
        height: auto;
        min-height: 60vh;
        padding: 40px 0;
    }
    
    .frame-content {
        flex-wrap: wrap;
        gap: 30px;
        justify-content: flex-start;
    }
    
    .services, .support, .company, .legal {
        width: calc(50% - 15px);
        min-width: 200px;
    }
    
    .subcribe {
        width: 100%;
        margin-top: 20px;
        padding-top: 20px;
        border-top: 1px solid rgba(255, 255, 255, 0.1);
    }
}

@media (max-width: 768px) {
    .frame {
        padding: 30px 0;
    }
    
    .frame-header {
        justify-content: center;
        margin-bottom: 30px;
    }
    
    .frame-header img {
        max-width: 150px;
    }
    
    .frame-content {
        flex-direction: column;
        align-items: center;
        gap: 35px;
    }
    
    .services, .support, .company, .legal {
        width: 100%;
        text-align: center;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    
    ul {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 15px;
    }
    
    li {
        margin-bottom: 0;
        font-size: 14px;
        padding: 0 10px;
    }
    
    h1 {
        font-size: 16px;
    }
    
    .subcribe {
        text-align: center;
        max-width: 400px;
    }
    
    .subcribe p {
        font-size: 14px;
        margin-bottom: 15px;
    }
}

@media (max-width: 480px) {
    .frame {
        padding: 25px 15px;
    }
    
    .frame-header, .frame-content {
        width: 95%;
    }
    
    h1 {
        font-size: 14px;
    }
    
    li {
        font-size: 13px;
    }
    
    ul {
        gap: 10px;
    }
    
    .subcribe p {
        font-size: 13px;
    }
}

</style>