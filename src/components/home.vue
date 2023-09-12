<template>
    <main class="wrapper">
        <section class="featured-box" id="home">
            <div class="featured-text">
                <div class="featured-name">
                    <p>I'm <span class="typedText"></span></p>
                </div>
                <div class="featured-text-info">
                    <p class="text-primary">FrontEnd</p>
                    <div class="featured-text-info-s">
                        <p class="text-secundary"> Developer</p>
                        <div class="featured-text-btn">
                            <button class="btn blue-btn">Hire me</button>
                            <a href="../../public/devfrontcurriculo.pdf" class="btn" download> <!-- Adicione o atributo "download" aqui -->
                                Download CV
                            </a>
                </div>
                    </div>
                    
                </div>
            </div>
            <div class="feature-image">
                <div class="image">
                    <img src="../assets/main.png" alt="Avatar">
                </div>
            </div>
        </section>
    </main>
</template>

<script>
    import Typed from 'typed.js';

    export default {
        name: 'HomeComponent',
        mounted(){
            new Typed(".typedText", {
                strings: ["José Carvalho", "student of s.i", "Developer"],
                loop: true,
                typeSpeed: 100,
                backSpeed: 80,
                backDelay: 2000
            });
        }
    }
</script>

<style scoped>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
}

.btn{
    padding: 12px 20px;
    background: #EEEEEE;
    color: #053B50;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    transition: .4s;
}

.btn>i{
    margin-left: 10px;
}

.btn:hover{
    background:#64CCC5;
    color: #eeeeee;
}

.featured-box{
    position: relative;
    display: flex;
    height: 100vh;
    min-height: 700px;
}

.featured-text{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 80vh;
    flex-direction: column;
    width: 50%;
    padding-left: 20px;
}

.featured-name{
    font-size: 50px;
    font-weight: 600;
    color: #053B50;
    margin-block: 15px;
}

.typedText{
    text-transform: capitalize;
    color: #64CCC5;
}

.featured-text-info{
    font-size: 15px;
    margin-bottom: 30px;
    color: #053B50;
}
.featured-text-info-s{
    display: flex;
    gap: 10px;
}
.text-primary{
    font-size: 80px;
}

.text-secundary{
    display: flex;
    font-size: 20px;
}

.featured-text-btn{
    display: flex;
    gap: 10px;
}
.featured-text-btn a {
    text-decoration: none;
    color: #053B50;
}

.featured-text-btn>.blue-btn{
    background-color: #EEEEEE;
    color: #053B50;
}
.featured-text-btn>.blue-btn:hover{
    background: #64CCC5;
    color: #EEEEEE;
}

.social_icons{
    display: flex;
    margin-left: 1em;
    gap: 10px;
}

.icon{
    color: #053B50;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 25px;
    height: 25px;
    border-radius: 50%;
    box-shadow: 0px 2px 5px 0px rgba(0, 0, 0, 0.25);
    cursor: point;
}
.icon:hover{
    color: #64CCC5;
    transition: 0.5s;
    transform: translateY(-7px);
}

/* FEATURED IMAGE BOX */

.feature-image{
    display: flex;
    justify-content: center;
    align-content: center;
    min-height: 80vh;
    width: 50%;
}
.image{
    margin: auto 0;
    width: 350px;
    height: 350px;
    animation: imgFloat 7s ease-in-out infinite;

    border-radius: 50%;
    box-shadow: 0px 2px 5px 0px rgba(0, 0, 0, 0.25);
    background: #053B50;
}
.image img{
    width: 480px;
    height: 480px;
    object-fit: contain;
}
@keyframes imgFloat {
    50%{
        transform: translateY(12px);
    }
}
</style>