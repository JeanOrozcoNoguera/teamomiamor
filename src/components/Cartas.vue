<template>
  <v-container fluid>
    <v-row
      style="padding-top: 10%; padding-bottom: 10%"
      v-for="carta in cartas"
      :key="carta.id"
      :style="'background-color:' + carta.color + ';'"
      justify="center"
    >
      <v-row justify="center">
        <v-col cols="10" md="8">
          <v-card
            elevation="0"
            style="border-radius: 20px"
            v-if="carta.posicion == 1"
          >
            <v-card-text>
              <v-row>
                <v-col cols="12" md="5">
                  <center>
                    <div>
                      <v-img
                        width="300"
                        style="border-radius: 20px"
                        :src="carta.url"
                      ></v-img>
                    </div>
                  </center>
                </v-col>
                <v-col cols="12" md="7">
                  <center>
                    <v-row>
                      <v-col cols="12">
                        <div style="padding: 30px">
                          <p class="parrafo">{{ carta.texto1 }}</p>
                        </div>
                      </v-col>
                      <v-col cols="12">
                        <p class="parrafoComentarios">{{ carta.texto2 }}</p>
                      </v-col>
                    </v-row>
                  </center>
                </v-col>
              </v-row>
            </v-card-text>
          </v-card>
          <v-card style="border-radius: 20px" elevation="0" v-if="carta.posicion == 2">
            <v-card-text>
              <v-row>
                <v-col cols="12" md="7">
                  <center>
                    <v-col cols="12">
                      <div style="padding: 30px">
                        <p class="parrafo">{{ carta.texto1 }}</p>
                      </div>
                    </v-col>

                    <v-col cols="12">
                      <p class="parrafoComentarios">{{ carta.texto2 }}</p>
                    </v-col>
                  </center>
                </v-col>
                <v-col cols="12" md="5">
                  <div>
                    <center>
                      <v-img
                        width="300"
                        style="border-radius: 20px"
                        :src="carta.url"
                      ></v-img>
                    </center>
                  </div>
                </v-col>
              </v-row>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-row>
  </v-container>
</template>
<script>
export default {
  data: () => ({
    cartas: [
      {
        id: 1,
        color: "#FFED63",
        posicion: "1",
        url: "/imagenes/foto1.jpeg",
        texto1: `
        Te doy las gracias siempre y esta vez no será la excepción, para mi es muy importante
        que siempre tengas presente que estoy agradecido por el aporte que has hecho en mi
        vida, sin duda alguna eres una persona muy pero muy diferente a TODAS las que conocí
        antes, y eso te lo agradezco hoy y lo haré siempre que tenga la oportunidad.
        Te doy las gracias por eso y por darme tanto cariño, por cuidarme, por preocuparte por mi
        por hacerme sentir especial y por todas las cosas que sabes que yo sé que haces por mi.
        No quiero que te vayas nunca de mi vida. Gracias también por llenar muchos momentos de mi vida
        de felicidad, de verdad muchas gracias por ello.
        `,
        texto2: '"Eres una persona muy importante para mi vida"',
      },
      {
        id: 2,
        color: "white",
        posicion: "2",
        texto1: `De nuestros momentos vividos, no puedo elegir un favorito, todos lo son.
        Sin embargo, mis momentos más preciados a tu lado son cuando te veo sonreir, sin duda alguna, es algo
        que disfruto mucho, que me confirma siempre que quiero verte feliz, que me hace feliz a mi el hecho que tu lo seas
        que tu sonrisa es una de las mejores cosas que me pasó. Que quiero luchar todos los días por esa sonrisa, que te amo
        y que te quiero amar por siempre. Que no tengo duda alguna de lo que siento por ti y que disfruto mucho y cada vez más
        tu sonrisa, a ti, todo de ti.`,
        texto2: '"Te amo, amo tu sonrisa, amo todo de ti"',
        url: "/imagenes/foto2.jpeg",
      },
      {
        id: 3,
        color: "#FFED63",
        posicion: "1",
        texto1: `Para mi, la vida hizo un excelente trabajo el día que me dio la oportunidad de conocerte, sabes que fue muy
        extraño como pasó todo, sin duda fue algo muy inesperado, aún así fue una casualidad hermosa, que agradezco siempre,
        me noté indiferente contigo, sin saber lo importante que llegarías a ser para mi y para mi vida en general.
        No sé que será de mi ahora en adelante, pero sin duda alguna quiero que estés tu ahí, acompañandome y que te sientas
        orgullosa de mi.`,
        texto2: '"Has sido mi apoyo inesperado y el más hermoso"',
        url: "/imagenes/foto3.jpeg",
      },
      {
        id: 4,
        color: "white",
        posicion: "2",
        texto1: `Igualmente me encantaría que cada paso que subas en la vida esté yo ahí para recordarte que puedes con
        todo, que me siento muy orgulloso de ti por todo lo que has logrado en la vida, porque nunca te rindes, porque lo que
        quieres lo consigues, porque eres fuerte, porque aunque tienes muchas cosas porque sufrir, no te detienen y sigues sonriendo
        porque no dudas nunca en ayudar a alguien, por ser buena persona, porque no dejas que tus miedos te frustren, porque eres
        una mujer excepcional y una maravillosa persona.`,
        texto2: '"Estoy muy orgulloso de ti, sigue luchando por tus sueños"',
        url: "/imagenes/foto4.jpeg",
      },
      {
        id: 5,
        color: "#FFED63",
        posicion: "1",
        texto1: `Si me pidieran una palabra para describir lo nuestro, creo que sería "MAGICO", porque sin ser perfecto,
        es algo que me hace feliz, porque es como de otro mundo, porque me lleva a mi a otra realidad, porque me quita los miedos
        porque de repente sonries y todo cambia para bien, porque aunque tenemos problemas, como cualquier mago, luchamos a nuestra
        manera para que cada día sea mejor, porque no queremos rendirnos, porque me ayudas y te ayudo, porque es magico, como lo que
        todos quieren en su vida, y pocos tienen la fortuna de conseguirlo.`,
        texto2: '"Cuando estoy contigo me siento en otra realidad, soy feliz."',
        url: "/imagenes/foto5.jpeg",
      },
      {
        id: 7,
        color: "white",
        posicion: "2",
        texto1: `Me gusta mucho la forma tan peculiar que tienes de vivir la vida, me gustan mucho tus locuras, tus risas a carcajadas
        tus caras extrañas, tus coqueteos, tu forma de hacer las cosas, el amor que le pones, me gusta que me cuides y que te preocupes
        por mi aún cuando no estás en todos tus sentidos, me gusta que seas tu en todos los momentos, que no ocultes nada de ti, me gusta que
        no le temas a nada y que si le temes a algo ni se note, me gusta que vayas por la vida persiguiendo tus sueños, que no te desmotive casi nada
        que seas dueña de tu risa, dueña de tus acciones y que NUNCA se vean mandadas por una situación o una persona.`,
        texto2: '"Me encanta tu persona en todas sus fases, más que nada porque nunca dejas de ser tu"',
        url: "/imagenes/foto7.jpeg",
      },
      {
        id: 8,
        color: "#FFED63",
        posicion: "1",
        texto1: `De todas las personas con las que pude coincidir en la vida, agradezco tanto de haber coincidido contigo
        nunca me cansaré de decirlo, eres una mujer excepcional, llena de muchas virtudes (aquí no hablaré de nada por mejorar)
        que es capas de conseguir muchas cosas, que tiene un excelente futuro por delante, que maneja muy bien los tiempo
        que no se desespera en situaciones complicadas y que esa calma que tiene le ayuda a conseguir todo lo que desea, me has enseñado
        cosas, cosas que no sé si otra persona me fuera podido enseñar, hey, es que eres espectacular, de verdad, me encantas,
        siempre que pueda te lo voy a recordar para que nunca se te olvide. Vivir contigo en su vida, sin duda alguna es un PLUS`,
        texto2: '"Sumas en mi vida, sumas donde llegas, sumas donde estés."',
        url: "/imagenes/foto6.jpeg",
      },
      {
        id: 9,
        color: "white",
        posicion: "1",
        texto1: `Y por ultimo, bueno, nada, recordarte lo que ya sabes, TE AMO, vas a encontrar en mi el apoyo que necesites, 
        un amigo, un hermano, un novio, un compañero, lo que necesites, de verdad, te amo, con lo que has hecho, que no ha sido poco
        te mereces todo lo bueno de la vida, nunca me voy a cansar de hacerte ver la luz que eres, nunca, de verdad, una vez más, gracias
        por ser tan especial, es que, no mameeeeeess, que genial es tenerte en mi vida, nunca dudes en decirme si necesitas mi ayuda, ahí
        estaré para ti, no importa en que, ahí estaré.`,
        texto2: '"TE AMO MUCHO MI AMOR"',
        url: "/imagenes/foto8.jpeg",
      },
    ],
  }),
};
</script>
<style scoped>
.parrafoComentarios {
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
  font-size: 3vh;
  color: grey;
}

.parrafo {
  font-size: 23px;
}
</style>