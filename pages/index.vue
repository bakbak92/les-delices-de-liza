<template>
    <main>
        <div class="head">
            <div class="content-title">
                <div class="title">
                    <h2>Traiteur Marocain | Rouen</h2>
                    <h1>les délices de liza</h1>
                    <p>De l'authenticité marocaine en plein rouen</p>
                    <div class="content-btn">
                        <button class="btn">
                            Nous contacter
                        </button>
                    </div>
                </div>
            </div>
        </div>
        <div class="presentation">
            <h2>Notre cuisine</h2>
            <p>Nous proposons une cuisine marocaine authentique faite maison avec des produits de qualité, des magnifiques saveurs, et une variété de plat</p>
        </div>
        <div class="plats">
            <div class="content-img">
                <img src="../assets/img/couscous.jpeg" alt="">
                <p>COUSCOUS</p>
            </div>
            <div class="content-img">
                <img src="../assets/img/tajine.jpeg" alt="">
                <p>Tajine</p>
            </div>
            <div class="content-img">
                <img src="../assets/img/soupe.jpeg" alt="">
                <p>Soupe</p>
            </div>
            <div class="content-img">
                <img src="../assets/img/wrap.jpeg" alt="">
                <p>Wrap</p>
            </div>
        </div>
        <div class="services">
            <h2>Nos services</h2>
            <p>Le Maroc est à l'honneur pour tous types d'événements : fêtes de comité d'entreprise , les déjeuners d'affaires, les anniversaires , ou tout autres évenements ...</p>
        </div>
        <section id="contact-times">
            <div class="times">
                <h2>Nos horraires d'ouverture</h2>
                <div class="content-time">
                    <div>
                        <div class="time">
                            <div class="day">Lundi</div>
                            <div class="hour">
                                Fermée
                            </div>
                        </div>
                        <div class="time">
                            <div class="day">Mardi</div>
                            <div class="hour">
                                11h - 20h
                            </div>
                        </div>
                        <div class="time">
                            <div class="day">Mercredi</div>
                            <div class="hour">
                                11h - 20h
                            </div>
                        </div>
                        <div class="time">
                            <div class="day">Jeudi</div>
                            <div class="hour">
                                11h - 20h
                            </div>
                        </div>
                        <div class="time">
                            <div class="day">Vendredi</div>
                            <div class="hour">
                                11h - 20h
                            </div>
                        </div>
                        <div class="time">
                            <div class="day">Samedi</div>
                            <div class="hour">
                                11h - 20h
                            </div>
                        </div>
                        <div class="time">
                            <div class="day">Dimanche</div>
                            <div class="hour">
                                11h - 20h
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="contact">
                <h2>Nous contacter</h2>
                <form>
                    <div class="content-input">
                        <input type="text" placeholder="Nom">
                    </div>
                    <div class="content-input">
                        <input type="email" placeholder="Email">
                    </div>
                    <div class="content-input">
                        <input type="tel" placeholder="Telephone">
                    </div>
                    <div class="content-input">
                        <textarea name="" id="" cols="30" rows="5" placeholder="Message"></textarea>
                    </div>
                    <div class="content-btn">
                        <button type="submit">Envoyer</button>
                    </div>
                </form>
            </div>
        </section>
    </main>
</template>

<script>
export default {}
</script>
<style lang="scss">
@import "../assets/css/colors.scss";
body{
    margin: 0;
    font-family: 'Lato', sans-serif;
    main{
        .head{
            background-image: url("../assets/img/plat-head.jpg");
            background-size: cover;
            height: 600px;
            padding: 30px;
            .content-title{
                position: relative;
                display: flex;
                justify-content: center;
            }
            .title{
                background-color: rgba(0, 0, 0, 0.6);
                padding: 30px;
                margin-top: 50px;
                h2{
                    color: $gold;
                }
                h1{
                    color: white;
                    font-size: 60px;
                    text-transform: uppercase;
                    margin: 20px 0;
                }
                p{
                    color: white;
                    font-size: 20px;
                }
                .btn{
                    background-color: $gold;
                    color: white;
                    border: none;
                    border-radius: 4px;
                    padding: 10px 40px;
                    font-size: 16px;
                }
                .content-btn{
                    text-align: center;
                }
            }
        }
        .presentation{
            text-align: center;
            p{
                font-size: 18px;
            }
        }
        .plats{
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            margin-left: 60px;
            .content-img{
                margin-right: 60px;
                text-align: center;
                text-transform: uppercase;
                img{
                    width: 100%;
                    height: 300px;
                }
            }
            @media screen and (max-width: 1200px){
                grid-template-columns: repeat(2, 1fr);
            }
            @media screen and (max-width: 700px){
                grid-template-columns: repeat(1, 1fr);
            }
        }
        .services{
            background-color: #EFE8D6;
            padding: 20px;
            text-align: center;
            h2{
                color: $gold;
            }
            p{
                color: #3B3427;
                font-size: 18px;
            }
        }
        #contact-times{
            display: grid;
            grid-template-columns: 1fr 1fr;
            max-width: 80%;
            margin: 0 auto;
            .times{
                h2{
                    color: $gold;
                }
                .content-time{
                    font-weight: 600;
                    .time{
                        display: flex;
                        margin-bottom: 20px;
                        .hour{
                            color: $gold;
                        }
                        div{
                            width: 100%;
                        }
                    }
                }
            }
            .contact{
                .content-input{
                    margin-bottom: 20px;
                    input{
                        border: 1px solid #D1D5DA;
                        border-radius: 4px;
                        line-height: 30px; 
                        width: 100%;
                        padding: 0 10px;
                    }
                    textarea{
                        border: 1px solid #D1D5DA;
                        border-radius: 4px;
                        width: 100%;
                        padding: 0 10px;
                    }
                }
                .content-btn{
                    text-align: right;
                }
                button{
                    background-color: $gold;
                    color: white;
                    border: none;
                    border-radius: 4px;
                    padding: 10px 40px;
                    font-size: 16px;
                }
            }
            @media screen and (max-width: 700px){
                grid-template-columns: repeat(1, 1fr);
            }
        }
    }
}
</style>