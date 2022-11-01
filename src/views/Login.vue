<template>
  <v-app id="inspire">
    <v-content class="body">
      <v-container color="fill-height" >
        <v-row align="center" justify="center">
          <v-col cols="12" sm="8" md="8">
            <v-card class="elevation-12" color="hsla(200, 64%, 22%,0.9)" >
              <v-window v-model="step" >
                <v-window-item :value="1" >
                  <v-row >
                    <v-col cols="12" md="8">
                      <v-card-text class="mt-12" >
                        <h1
                          class="text-center display-2 color1 text--accent-3"
                        >Ingresa a <span>Viajes</span> & Hotelería</h1>
                        <div class="text-center mt-4">
                          <v-btn class="mx-2" fab color="rgb(0, 255, 255)" outlined>
                            <v-icon>fab fa-facebook-f</v-icon>
                          </v-btn>

                          <v-btn class="mx-2" fab color="rgb(0, 255, 255)" outlined>
                            <v-icon>fab fa-google-plus-g</v-icon>
                          </v-btn>
                          <v-btn class="mx-2" fab color="rgb(0, 255, 255)" outlined>
                            <v-icon>fab fa-linkedin-in</v-icon>
                          </v-btn>
                        </div>
                        <h4 class="text-center mt-4 color1 w-text">Ingresa tu correo electrónico para iniciar sesión</h4>
                        <v-form>
                          <v-text-field
                            label="Correo"
                            name="Correo"
                            prepend-icon="email"
                            type="email"
                            color="rgb(0, 255, 255)"
                          />

                          <v-text-field
                            id="contraseña"
                            label="contraseña"
                            name="password"
                            prepend-icon="lock"
                            type="password"
                            color="rgb(0, 255, 255)"
                          />
                        </v-form>
                        <h3 class="text-center mt-4 "> <a class="color1 w-text" href="">¿Olvidaste tu contraseña ?</a> </h3>
                      </v-card-text>
                      <div class="text-center mt-3 " >
                        <v-btn class="boton" rounded color="rgb(0, 255, 255)" dark><p class="color-p">Iniciar Sesión</p></v-btn>
                      </div>
                    </v-col>
                    <v-col cols="12" md="4" class="white accent-3">
                      <v-card-text class="primary__color mt-12">
                        <h1 class="text-center color__cyan display-1">Hola, Bienvenido!</h1>
                        <h5
                          class="text-center w-text1"
                        >Ingresa tus datos personales y comience a viajar con nosotros</h5>
                      </v-card-text>
                      <div class="text-center container-ins">
                        <v-btn class="boton-ins" rounded outlined dark color="hsla(200, 64%, 22%)" @click="step++">INSCRÍBETE</v-btn>
                        <a href=""><img class="logo" src="./../assets/img/logo1.png" alt="" ></a>
                      </div>
                    </v-col>
                  </v-row>
                </v-window-item>
                <v-window-item :value="2">
                  <v-row class="fill-height">
                    <v-col cols="12" md="4" class="white accent-3">
                      <v-card-text class="primary__color mt-12">
                        <h1 class="text-center display-1">¡Bienvenido de nuevo!</h1>
                        <h5
                          class="text-center w-text1"
                        >Para mantenerser conectado con nosotros, inicie sesión con tu información personal</h5>
                      </v-card-text>
                      <div class="text-center container-ins">
                        <v-btn rounded outlined dark  color="hsla(200, 64%, 22%)" @click="step--">Inicia Sesión</v-btn>
                        <a href=""><img class="logo" src="./../assets/img/logo1.png" alt="" ></a>
                      </div>
                    </v-col>

                    <v-col cols="12" md="8">
                      <v-card-text class="mt-12">
                        <h1 class="text-center display-2 color1 text--accent-3">Crar Cuenta</h1>
                        <div class="text-center mt-4">
                          <v-btn class="mx-2" fab color="rgb(0, 255, 255)" outlined>
                            <v-icon>fab fa-facebook-f</v-icon>
                          </v-btn>

                          <v-btn class="mx-2" fab color="rgb(0, 255, 255)" outlined>
                            <v-icon>fab fa-google-plus-g</v-icon>
                          </v-btn>
                          <v-btn class="mx-2" fab color="rgb(0, 255, 255)" outlined>
                            <v-icon>fab fa-linkedin-in</v-icon>
                          </v-btn>
                        </div>
                        <h4 class="text-center mt-4 color1 w-text">Ingresa tu correo electrónico para el registro</h4>
                        <v-form>
                          <v-text-field
                            label="Nombre"
                            name="Nombre"
                            prepend-icon="person"
                            type="text"
                            color="rgb(0, 255, 255)"
                          />
                          <v-text-field
                            label="Correo"
                            name="Correo"
                            prepend-icon="email"
                            type="email"
                            color="rgb(0, 255, 255)"
                          />

                          <v-text-field
                            id="password"
                            label="Password"
                            name="password"
                            prepend-icon="lock"
                            type="password"
                            color="rgb(0, 255, 255)"
                          />
                        </v-form>
                      </v-card-text>
                      <div class="text-center mt-n5">
                        <v-btn rounded color="rgb(0, 255, 255)" dark><p class="color-p">REGISTRARSE</p></v-btn>
                      </div>
                    </v-col>
                  </v-row>
                </v-window-item>
              </v-window>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    step: 1
  }),
  props: {
    source: String
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&family=Staatliches&display=swap");
a{
  text-decoration: none;
}
.body{
  margin: 0;
  padding: 0;
  background-image: url(./../assets/img/Caribbean.jpg);
  background-repeat:no-repeat;
  background-size: cover;
  position: relative;
  font-family:'Roboto', sans-serif;
  height: 100vh; 
}
.primary__color{
  color:hsla(200, 64%, 22%,1);
}
.color-p{
  margin-top: 15px;
  color:hsla(200, 64%, 22%,1);
}
.w-text{
  font-weight: lighter;
}
.w-text1{
  font-weight:normal;
  font-size: 0.75rem;
}
.color1{
  color: #fff;
}
.color1 span{
  color: rgb(0, 255, 255);
}
.color__cyan{
  color: rgb(23, 228, 228);
}
.color2{
  color:darkgray;
  }

[prepend-icon="password"]{
    color: #fff;
}
[type="email"],
[type="text"],
[type="password"]{
    border-bottom: 1px solid #fff;
}
.container-ins{
  display: flex;
  flex-direction: column;
  row-gap: 3rem;
  text-align: center;
}
.logo{
    width: 110px;
    height: 60px;

    
}
.boton-ins{
  height: 1rem;
}
</style>