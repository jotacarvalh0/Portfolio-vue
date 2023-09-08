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
                        <div class="social_icons">
                            <a href="#" class="icon"><svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor" class="bi bi-linkedin" viewBox="0 0 16 16"><path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z"/></svg></a>
                            <a href="#" class="icon"><svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor" class="bi bi-github" viewBox="0 0 16 16"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg></a>
                        </div>
                    </div>
                    
                </div>
                <div class="featured-text-btn">
                            <button class="btn blue-btn">Hire me</button>
                            <button class="btn">Download CV
                            <i class="uil uil-file-alt"></i></button> <!--Adicionar icones nos I-->
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