<template>
    <v-container fluid>
        <v-row class="contenedor">
            <v-col col="12" md="5">
                <div class="contenedor_img">
                    <v-img width="500"  src="../../src/assets/icons/bienvenida.svg"></v-img>
                </div>
            </v-col>
            <v-col cols="12" md="7" class="contenedor_texto">
                <div class="parrafo">
                    <p class="saludo">HOLA,</p>
                    <span class="saludo2">ESTO LO HICE CON MUCHO</span> <br>
                    <span class="mi_amor">AMOR PARA TI.</span>
                    
                    <p>
                        <br> <br>
                        <v-btn color="#FFED63" icon large >
                            <v-icon size="100"> mdi-chevron-double-down</v-icon>
                        </v-btn>
                    </p>
                </div>
            </v-col>
        </v-row>
    </v-container>
</template>
<style scoped>
.parrafo {
    text-align: right;
    padding-top:15%;
}
.saludo {
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: 10vh;
    color:grey;
    margin: 0;
    padding:0;
    line-height : 80px;
}

.saludo2 {
    font-size: 7vh;
    /* line-height : 60px; */
    margin: 0;
    padding:0;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    
}

.mi_amor {
    font-size: 90px;
    line-height : 60px;
    color:#FFED63;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}

.contenedor {
    padding-top: 10%;
    color:grey;
    height: 100vh;
}

.contenedor_img {
    padding-left: 10%;
}

.contenedor_texto {
    padding-right: 10%;
    margin-bottom: 50px;
}
</style>