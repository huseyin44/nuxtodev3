<template>
  <div id="anasayfa">
   <div class="test">%100 Orijinal • Ücretsiz Kargo • Vade Farksız 9 Taksit </div>
   <v-container class="birincisatir" fluid>
     <v-row >
       <v-col>
         <nuxt-link to="/">
         <v-img class="saat" src="https://cdn.saatvesaat.com.tr/skin/frontend/base/default/images/new-logo.png"/>
         </nuxt-link>
       </v-col>
       <v-col class="buton1">BAYAN SAAT</v-col>
       <v-col class="buton1">ERKEK SAAT</v-col>
       <v-col class="buton1">ÇOCUK SAAT</v-col>
       <v-col class="buton10">
        <v-row justify="center" >
         <v-menu v-model="showMenu3" offset-y open-on-hover >
      <template v-slot:activator="{ on, attrs }"  > 
        <div v-bind="attrs"  v-on="on" >
        MARKALAR
        </div>
      </template>
      <v-list class="itemlistelemecolumn">
        <div :class="{ red3 : gecersiz3 }" @mouseover="kirmizi3" @mouseleave="gecersiz3=false">
        88 Rue Du Rhone
        </div>
      <nuxt-link to="/MarkaClick"  style="text-decoration: none; color: inherit;">
      <div :class="{ red4 : gecersiz4 }" @mouseover="kirmizi4" @mouseleave="gecersiz4=false">Armani Exchange </div>
      </nuxt-link>
      <div :class="{ red5 : gecersiz5 }" @mouseover="kirmizi5" @mouseleave="gecersiz5=false">Bomberg </div>
      <div :class="{ red6 : gecersiz6 }" @mouseover="kirmizi6" @mouseleave="gecersiz6=false">Boss Watches </div>
      <div :class="{ red7 : gecersiz7 }" @mouseover="kirmizi7" @mouseleave="gecersiz7=false">DKNY </div>
      <div>Edox </div>
      <div>Empori Armani </div>
      <div>Escape  </div>
      <div>Esprit  </div>
      <div>FENDI </div>
      <div>Fossil</div>
      <div>Gc </div>
      <div>Glam Rock </div>
      <div>Guess </div>
      <div>Lacoste </div>
      <div>Lorus </div>
      <div>Oris </div>
      <div>Parigi </div>
      <div>Seiko </div>
      <div>Skagen </div>
      <div>Skechers </div>
      <div>Tag HEUER </div>
      <div>Thom Olson </div>
      <div>Young Sterna </div>
      <div>Xonix </div>
      </v-list>
         </v-menu> 
         </v-row>
       </v-col>
       <v-col class="buton2">TAKI & AKSESUAR</v-col>
       <v-col class="buton4">FIRSAT</v-col>
       <v-col class="buton3">ONLİNE ÖZEL</v-col>
       <v-col class="aramaa">
         <div>
          <input class="arama2" type="search" placeholder="Kelime / Kod" autocomplete="off">
          <input class="arares" type="image" src="https://www.flaticon.com/svg/static/icons/svg/622/622669.svg" >
        </div>
      </v-col>
      <v-col class="buton7" >  
         <v-row justify="center" class="test2">
          <v-menu v-model="showMenu" offset-y >
           <template v-slot:activator="{ on, attrs }">
             <v-card
              img="https://www.flaticon.com/svg/static/icons/svg/747/747376.svg"
              height="30"
              width="30"
              v-bind="attrs"
              v-on="on">
            </v-card>
           </template>
           <v-list>
            <div :class="{ red9 : gecersiz9 }" @mouseover="kirmizi9" @mouseleave="gecersiz9=false">Favori Listem</div>
            <div :class="{ red10 : gecersiz10 }" @mouseover="kirmizi10" @mouseleave="gecersiz10=false">Sepetim</div>
            <div :class="{ red11 : gecersiz11 }" @mouseover="kirmizi11" @mouseleave="gecersiz11=false">Alışverişi Tamamla</div>
            <div :class="{ red12 : gecersiz12 }" @mouseover="kirmizi12" @mouseleave="gecersiz12=false" >
             <nuxt-link to="/Giris"  style="text-decoration: none; color: inherit;">Giris</nuxt-link>
             </div>
            <div :class="{ red13 : gecersiz13 }" @mouseover="kirmizi13" @mouseleave="gecersiz13=false">Üye Ol</div>
          </v-list>
          </v-menu>
         </v-row>
      </v-col>
      <v-col class="buton7"> 
         <v-row justify="center" class="test2" >
          <v-menu v-model="showMenu2" offset-y >
           <template v-slot:activator="{ on, attrs }">
             <v-card
              img="https://www.flaticon.com/svg/static/icons/svg/126/126515.svg"
              height="30"
              width="30"
              v-bind="attrs"
              v-on="on">
            </v-card>
           </template>
           <v-list>
            <div>Sepet</div>
            <div>Sepetiniz Boş </div>
          </v-list>
          </v-menu>
         </v-row>
      </v-col>
     </v-row>
   </v-container>
  </div>
</template>

<script>
export default {
data: () => ({
    showMenu: false,
    showMenu2: false,
    showMenu3: false,
    gecersiz1: false,
    gecersiz2: false,
    gecersiz3: false,
    gecersiz4: false,
    gecersiz5: false,
    gecersiz6: false,
    gecersiz7: false,
    gecersiz9: false,
    gecersiz10: false,
    gecersiz11: false,
    gecersiz12: false,
    gecersiz13: false,
  }),
  methods:{
       kirmizi9() {
      this.gecersiz9= true;
  },
   kirmizi10() {
      this.gecersiz10= true;
  },
   kirmizi11() {
      this.gecersiz11 = true;
  },
   kirmizi12() {
      this.gecersiz12 = true;
  },
   kirmizi13() {
      this.gecersiz13 = true;
  },
  kirmizi1() {
      this.gecersiz1 = true;
  },
  kirmizi2() {
      this.gecersiz2 = true;
  },
   kirmizi3() {
      this.gecersiz3 = true;
  },
   kirmizi4() {
      this.gecersiz4 = true;
  },
   kirmizi5() {
      this.gecersiz5 = true;
  },
   kirmizi6() {
      this.gecersiz6 = true;
  },
   kirmizi7() {
      this.gecersiz7 = true;
  },
  }
}
</script>

<style scoped>
.test{
 background: black;
 color: white;
 text-align: center
}
.birincisatir{
  background: #F9F9F9;
  height: 70px;
  width: 1500px;
}
.saat{
  height: 40px;
  width:170px;
  bottom: 10px;
}
.buton10{
  max-width: 100px;
  height: 60px;
  white-space: nowrap;
  color: #353535;
  font-size: 16px;
}
.buton1{
  max-width: 120px;
  height: 60px;
  white-space: nowrap;
  color: #353535;
  font-size: 16px;
}
.buton2{
  height: 60px;
  white-space: nowrap;
  max-width: 150px;
  color: #353535;
  font-size: 16px;
}
.buton3{
  width: 80px;
  height: 60px;
  max-width: 120px;
  white-space: nowrap;
  color: #BD1818;
  font-size: 16px;
}
.buton4{
  height: 60px;
  max-width: 70px;
  color: #353535;
  font-size: 16px;
}
.aramaa{
  position: relative;
  padding-top: 0;
  width: 240px;
  height: 32px;
  top: 8px;
  border-radius: 70px/90px;
  background: white;
  border-style: solid;
  border-color: rgb(231, 231, 231);
}
.arama2{
  width: 140px;
  height: 32px;
  padding-right: 40px;
  font-family: "Roboto", Arial, sans-serif;
  border-radius: 30px;
  font-size: 12px;
}
.arares{
  text-indent: -9999px;
  position: absolute;
  top: 0;
  right: 0;
  width: 27px;
  height: 20px;
  top: 3px;
  border: 0;
  background: none;
}
.buton7{
  max-width: 117px;
  height: 60px;
}
.test2{
 background: #F9F9F9;
 max-height: 45px;
}
.red3{
  color: red;
}
.red4{
  color: red;
}
.red5{
  color: red;
}
.red6{
  color: red;
}
.red7{
  color: red;
}
.red9{
  color: red;
  text-decoration: underline;
}
.red10 {
  color: red;text-decoration: underline;
}
.red11 {
  color: red;text-decoration: underline;
}
.red12 {
  color: red;text-decoration: underline;
}
.red13 {
  color: red;text-decoration: underline;
}
.itemlistelemecolumn{
  column-count: 3;
}
.test2:hover{
  background: #BD1818;
}
</style>