<template>
  <v-app>
    <v-main>
    <h1>Menu Principal</h1>
     <MenuPrincipal/>
     <!-- <h1>Carrusel</h1>
     <CarouselsAll/>
    <h1>Botones</h1>
     <BotonesAll/>
     <h1>Button Groups</h1>
     <ButtonGroupsAll/>
     <h1>Paneles expansion</h1>
     <PanelesExpansionAll/>
    <h1>Calendario</h1>
     <CalendarioAll/>
     <h1>Dialogo</h1>
     <DialogoAll/>
    <h1>Footer</h1>
     <FooterAll/> -->
    <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
import MenuPrincipal from './components/MenuPrincipal';
/* import CarouselsAll from './components/CarouselsAll';
import BotonesAll from './components/BotonesAll';
import ButtonGroupsAll from './components/ButtonGroupsAll';
import PanelesExpansionAll from './components/PanelesExpansionAll';
import CalendarioAll from './components/CalendarioAll';
import DialogoAll from './components/DialogoAll';
import FooterAll from './components/FooterAll'; */

export default {
  name: 'App',

  components: {
    MenuPrincipal,
    /* CarouselsAll,
    BotonesAll,
    ButtonGroupsAll,
    PanelesExpansionAll,
    CalendarioAll,
    DialogoAll,
    FooterAll, */
    
  },

  data: () => ({
    //
  }),
};
</script>
