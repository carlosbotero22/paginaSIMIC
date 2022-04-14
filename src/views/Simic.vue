// *********************
// *** CARLOS BOTERO ***
// *********************

<template>
<div class="container">
    <div class="header">
        <v-app-bar style="background: linear-gradient(to right, DarkCyan, SteelBlue, DarkCyan);">
            <v-row>
                <v-dialog v-model="dialog" persistent max-width="600px">
                    <template v-slot:activator="{ on, attrs }">
                        <v-btn @click="dialog = true" elevation="2" color="white" border="1px solid #FDFDFD" dark v-bind="attrs" v-on="on">
                            Consulta
                        </v-btn>
                    </template>
                    <v-card>
                        <v-card-title>
                            <span class="text-h5">INGRESA LOS DATOS DE USUARIO</span>
                        </v-card-title>
                        <v-card-text>
                            <v-container>
                                <v-row>
                                    <v-col cols="12" sm="6" md="4">
                                        <v-text-field label="Nombres:*" required></v-text-field>
                                    </v-col>
                                    <v-col cols="12" sm="6" md="4">
                                        <v-text-field label="Apellidos:" hint="example of helper text only on focus"></v-text-field>
                                    </v-col>
                                    <v-col cols="12" sm="6" md="4">
                                        <v-text-field label="identificación:*" hint="example of persistent helper text" persistent-hint required></v-text-field>
                                    </v-col>
                                    <v-col cols="12" sm="6">
                                        <v-select :items="['0-17', '18-29', '30-54', '54+']" label="Edad*" required></v-select>
                                    </v-col>
                                    <v-col cols="12" sm="6">
                                        <v-autocomplete :items="['Skiing', 'Ice hockey', 'Soccer', 'Basketball', 'Hockey', 'Reading', 'Writing', 'Coding', 'Basejump']" label="interés" multiple></v-autocomplete>
                                    </v-col>
                                </v-row>
                            </v-container>
                            <small>*indicates required field</small>
                        </v-card-text>
                        <v-card-actions>
                            <v-spacer></v-spacer>
                            <v-btn color="blue darken-1" text @click="dialog = false">
                                Cerrar
                            </v-btn>
                            <v-btn color="blue darken-1" text @click="dialog = false">
                                Guardar
                            </v-btn>
                        </v-card-actions>
                    </v-card>
                </v-dialog>
            </v-row>

        </v-app-bar>

        <div class="fotos">
            <v-carousel>
                <v-carousel-item v-for="(item,i) in items" :key="i" :src="item.src" reverse-transition="fade-transition" transition="fade-transition"></v-carousel-item>
            </v-carousel>
        </div>
    </div>

    <div class="body">
        <div class="slider">
            <div class="slider-track">
                <div class="slide">
                    <img src="s1.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="5.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="1.png" alt="" height="100" width="250">
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
                    <img src="1.png" alt="" height="100" width="250">
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
                    <img src="1.png" alt="" height="100" width="250">
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
                    <img src="1.png" alt="" height="100" width="250">
                </div>
                <div class="slide">
                    <img src="neiva.png" alt="" height="100" width="250">
                </div>
            </div>
        </div>

        <div class="galeria">
            <div class="galeria">
                <h2 class="subtitulo">Nuestro servicio</h2>
                <div class="servicios">
                    <img class="imagen" src="https://img.freepik.com/vector-gratis/gente-moderna-haciendo-actividades-culturales_52683-42205.jpg?t=st=1648584624~exp=1648585224~hmac=88ac542e258d1691aa2f0e884fdaac821951092c29ffe2f36c4bb6ba79dca5ea&w=740" alt="">
                    <div class="con-servicio">
                        <div class="sub">
                            <h2 class="titu">OBJETIVO</h2>
                            <p class="pa">Promover el desarrollo cultural que involucre todas las manifestaciones culturales y artísticas que hacen parte de nuestra identidad local y regional generando cambios en el comportamiento de los ciudadanos reflejados en la formación de principios y valores y el respeto por lo público.</p>
                            <h2 class="titu">MISIÓN</h2>
                            <p class="pa">La Secretaría de Cultura está encargada de fijar la política cultural del Municipio de Neiva y establecer las estrategias que hagan transversalidad y coherencia con las políticas nacionales y departamentales articulando los sectores socioeconómicos del país. Igualmente deberá impulsar las formas de expresión y la defensa del patrimonio cultural del Municipio.</p>
                        </div>
                    </div>
                </div>
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
    height: 120px;
    margin: auto;
    margin-top:30px;
    overflow: hidden;
    position: relative;
    width: 60%;
    
}

.slider-track {
    animation: scroll 40s linear infinite;
    display: flex;
    width: calc(250px * 7);
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

.subtitulo {
    text-align: center;
    font-weight: 300;
    color: #026167;
    margin-bottom:40px;
    font-size: 40px;
    
}

.servicios {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    flex-wrap: wrap;
}

.sub {
    text-align:center;
}

.titu {
    padding:10px;
}

.imagen {
    width: 30%;
    margin-bottom: 60px;
}

.pa {
    color: #026167;
}

h2 {
    font-size: 30px;
    color: #026167;
}

.con-servicio {
    width: 40%;
    margin-bottom: 70px;
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

@keyframes burbujas {
    0% {
        bottom: 0;
        opacity: 0;
    }

    30% {
        transform: translateX(30px);
    }

    100% {
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
            dialog: false,
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
