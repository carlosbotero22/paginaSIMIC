// *********************
// *** CARLOS BOTERO ***
// *********************

<template>
<div class="container">
    <div class="header">
        <v-app-bar style="background: linear-gradient(to right, DarkCyan, SteelBlue, DarkCyan);">
            <v-btn color="white" elevation="4">CONSULTA</v-btn>
        </v-app-bar>

        <div class="fotos">
            <v-carousel>
                <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.src" reverse-transition="fade-transition" transition="fade-transition"></v-carousel-item>
            </v-carousel>
        </div>
    </div>

    <div class="body">
        <div class="slider">
            <h2> NOSOTROS </h2>

            <div class="slider-track">
                <div class="slide">
                    <img src="s1.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="5.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="n.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="neiva.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="s1.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="5.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="n.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="neiva.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="s1.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="5.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="n.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="neiva.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="s1.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="5.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="n.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="neiva.png" alt="" height="100" width="250">
                </div>
            </div>
        </div>

        <div class="galeria">
            <h3> GALERÍA </h3>
            <div class="fotos">
                <v-card class="mx-auto" max-width="400">
                    <v-img class="white--text align-end" height="200px" src="https://i0.wp.com/lagaceta.com.co/wp-content/uploads/2021/03/IMG-20210316-WA0048.jpg?resize=1024%2C683&ssl=1">
                        <v-card-title>Top 10 Australian beaches</v-card-title>
                    </v-img>

                    <v-card-subtitle class="pb-0">
                        Number 10
                    </v-card-subtitle>

                    <v-card-text class="text--primary">
                        <div>Whitehaven Beach</div>

                        <div>Whitsunday Island, Whitsunday Islands</div>
                    </v-card-text>

                    <v-card-actions>
                        <v-btn color="orange" text>
                            Share
                        </v-btn>

                        <v-btn color="orange" text>
                            Explore
                        </v-btn>
                    </v-card-actions>
                </v-card>
                <v-card class="mx-auto" max-width="400">
                    <v-img class="black--text align-end" height="200px" src="https://i0.wp.com/lagaceta.com.co/wp-content/uploads/2021/03/IMG-20210316-WA0048.jpg?resize=1024%2C683&ssl=1">
                        <v-card-title>Top 10 Australian beaches</v-card-title>
                    </v-img>

                    <v-card-subtitle class="pb-0">
                        Number 10
                    </v-card-subtitle>

                    <v-card-text class="text--primary">
                        <div>Whitehaven Beach</div>

                        <div>Whitsunday Island, Whitsunday Islands</div>
                    </v-card-text>

                    <v-card-actions>
                        <v-btn color="orange" text>
                            Share
                        </v-btn>

                        <v-btn color="orange" text>
                            Explore
                        </v-btn>
                    </v-card-actions>
                </v-card>
                <v-card class="mx-auto" max-width="400">
                    <v-img class="white--text align-end" height="200px" src="https://i0.wp.com/lagaceta.com.co/wp-content/uploads/2021/03/IMG-20210316-WA0048.jpg?resize=1024%2C683&ssl=1">
                        <v-card-title>Top 10 Australian beaches</v-card-title>
                    </v-img>

                    <v-card-subtitle class="pb-0">
                        Number 10
                    </v-card-subtitle>

                    <v-card-text class="text--primary">
                        <div>Whitehaven Beach</div>

                        <div>Whitsunday Island, Whitsunday Islands</div>
                    </v-card-text>

                    <v-card-actions>
                        <v-btn color="orange" text>
                            Share
                        </v-btn>

                        <v-btn color="orange" text>
                            Explore
                        </v-btn>
                    </v-card-actions>
                </v-card>
            </div>

        </div>

        <div class="geo">
            <div class="burbujas">
                <div class="burbuja"></div>
                <div class="burbuja"></div>
                <div class="burbuja"></div>
                <div class="burbuja"></div>
                <div class="burbuja"></div>
                <div class="burbuja"></div>
                <div class="burbuja"></div>

            </div>
            <div class="mapa">
                <img src="tablet.png" alt="" width="700" height="370" box-shadow="60px -16px teal">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3984.6068218000255!2d-75.29169418573697!3d2.928799655285659!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8e3b747c9970b24d%3A0x3fb1bbeb4af8f8a7!2sAlcald%C3%ADa%20de%20Neiva!5e0!3m2!1ses!2sco!4v1646626239750!5m2!1ses!2sco" width="348" height="200" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </div>
            <div class="texto">
                <h1>Geolocalización</h1>
                <P>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Itaque repellat repellendus illum tempore aliquam autem ad dolores. Eum quasi, unde doloremque maiores totam labore quia ad pariatur odit, dolores omnis et veritatis voluptates itaque optio aut esse voluptatum exercitationem iusto?</P>
                <div class="decor"></div>
            </div>

        </div>

        <div class="footer">
            <div class="fot">
                <h4>&copy; Copyright - Secretaría de TIC</h4>
            </div>
        </div>
    </div>
</div>
</template>

// *********************
// *** ESTILOS ***
// *********************

<style>
v-app-bar {
    position: sticky;
    top: 0%;
}

/* *** slide*** */
.slider {
    height: 200px;
    margin: auto;
    overflow: hidden;
    position: relative;
    width: 60%;
}

.slider-track {
    animation: scroll 40s linear infinite;
    display: flex;
    width: calc(250px * 7);
}

h2 {
    padding: 20px;
    font-size: 20px;
    text-align: center;
    font-family: Tahoma;

}

.slide {
    height: 100px;
    width: 250px;
    perspective: 130px;
}

img:hover {
    transform: translateZ(20px);
}

@keyframes scroll {
    0% {
        transform: translateX(0);
    }

    100% {
        transform: translateX(calc(-250px * 9));
    }
}

/* *** galeria *** */

.galeria {
    width: 100%;
    height: 80%;
    margin-top: 10px;
}

.fotos {
    margin-top: 40px;
    display: flex;
    justify-content: center;
}

v-card:hover {
    transform: scale(1.2);
}

h3 {
    color: black;
    font-size: 25px;
    text-align: center;
    font-family: Verdana;
}

/* *** geo *** */
.geo {
    width: 100%;
    height: 400px;
    padding: 10px;
    margin-top: 20px;
    position: relative;
    display: flex;
    background-image: url(/public/p2.jpg);
    width: 100%;
}

.burbuja {
    background: white;
    opacity: .5;
    position: absolute;
    border-radius: 50%;
    bottom: -150;
    z-index: 100%;
    animation: burbujas 3s linear infinite;
}

.burbuja:nth-child(1) {
    width: 20px;
    height: 20px;
    left: 5%;

    animation-duration: 2s;
    animation-delay: 3s;
}

.burbuja:nth-child(2) {
    width: 30px;
    height: 30px;
    left: 15%;

    animation-duration: 3s;
    animation-delay: 3s;
}

.burbuja:nth-child(3) {
    width: 40px;
    height: 40px;
    left: 25%;

    animation-duration: 2s;
    animation-delay: 5s;
}

.burbuja:nth-child(4) {
    width: 20px;
    height: 20px;
    left: 35%;

    animation-duration: 3s;
    animation-delay: 3s;
}

.burbuja:nth-child(5) {
    width: 10px;
    height: 10px;
    left: 45%;

    animation-duration: 2s;
    animation-delay: 5s;
}

.burbuja:nth-child(6) {
    width: 20px;
    height: 20px;
    left: 55%;

    animation-duration: 3s;
    animation-delay: 3s;
}

.burbuja:nth-child(7) {
    width: 30px;
    height: 30px;
    left: 65%;

    animation-duration: s;
    animation-delay: 5s;
}

.burbuja:nth-child(8) {
    width: 10px;
    height: 10px;
    left: 75%;

    animation-duration: 3s;
    animation-delay: 3s;
}

.burbuja:nth-child(9) {
    width: 30px;
    height: 30px;
    left: 85%;

    animation-duration: 3s;
    animation-delay: 5s;
}

.burbuja:nth-child(10) {
    width: 20px;
    height: 20px;
    left: 95%;

    animation-duration: 3s;
    animation-delay: 3s;
}

@keyframes burbujas{
    0%{
        bottom:0;
        opacity:0;
    }
    30%{
        transform: translateX(30px);
    }

    100%{
        bottom: 100vh;
    }
}

.texto {
    width: 45%;
    height: 220px;
    margin-top: 30px;
    margin-left: 80px;
    text-align: center;
    padding: 60px;
}

h1 {
    color: white;

}

h1:hover {
    transform: scale(1.2);
}

p {
    color: white;

}

p:hover {
    transform: scale(1.2);
}

.decor {
    padding: 10px;
    border-bottom: 5px solid;
    border-bottom-color: white;
}

.decor:hover {
    transform: scale(1.2);
}

.mapa {
    width: 45%;
    height: 100%;
    padding: 20px;
    position: relative;
}

img {
    margin-right: 40px;
}

iframe {
    top: 0;
    margin-top: 86px;
    margin-left: 180px;
    position: absolute;
    /* animation: tablet 5s linear infinite; */
}

@keyframes tablet {
    0% {
        bottom: 0;
        opacity: 0;
    }

    50% {
        opacity: .4;
    }

    100% {
        opacity: 100%;

    }

}

/* *** footer *** */
.footer {
    width: 100%;
    height: 50px;
    background-color: white;
}

h4 {
    color: black;
    margin-top: 25px;
    text-align: center;
}
</style>

// *********************
// *** SCRIPT ***
// *********************

<script>
export default {
    data() {

        return {
            show: false,
            items: [{
                    src: 'p1.jpg',
                },
                {
                    src: 'p3.jpg',
                },
                {
                    src: 'prin.jpg',
                },
                {
                    src: 'https://img.freepik.com/foto-gratis/huellas-manos-borde-multicolor_1101-2085.jpg?t=st=1648236256~exp=1648236856~hmac=7a6d6492cd48fa01ad094ffd984a1a820043e928f992ae8f9d544c051c1e86d5&w=996',
                },
            ],
        }
    },

}
</script>
