<template>
<div>
  <v-container class="satirbir" fluid>
    <v-row contain>
      <v-col>
        <v-row>
          <v-menu  open-on-hover offset-y  >
           <template v-slot:activator="{ on, attrs }">
            <div v-bind="attrs" v-on="on" class="buton1">
             Kategori
            </div>
            </template>
            <v-list class="kategorilist" >
             <div :class="{ red14 : gecersiz14 }" @mouseover="kirmizi14" @mouseleave="gecersiz14=false">Saat</div>
             <div :class="{ red15 : gecersiz15 }" @mouseover="kirmizi15" @mouseleave="gecersiz15=false">Fırsat</div>
             <div :class="{ red16 : gecersiz16 }" @mouseover="kirmizi16" @mouseleave="gecersiz16=false">Online-Mağazaya-Özel</div>
             <div :class="{ red17 : gecersiz17 }" @mouseover="kirmizi17" @mouseleave="gecersiz17=false" >İndirimli-Saatler </div>
            </v-list>
         </v-menu>
        </v-row>
      </v-col>
      <v-col>
       <v-row>
          <v-menu  open-on-hover offset-y  >
           <template v-slot:activator="{ on, attrs }">
            <div v-bind="attrs" v-on="on" class="buton1" >
             Cinsiyet
            </div>
            </template>
            <v-list class="kategorilist" >
             <v-radio :class="{ red18 : gecersiz18 }" @mouseover="kirmizi18" @mouseleave="gecersiz18=false" label="Erkek"></v-radio>
             <v-radio :class="{ red19 : gecersiz19 }" @mouseover="kirmizi19" @mouseleave="gecersiz19=false" label="Kadın"></v-radio>
            </v-list>
         </v-menu>
       </v-row>
      </v-col>
      <v-col>
        <v-row>
          <v-menu  open-on-hover offset-y  >
           <template v-slot:activator="{ on, attrs }">
            <div v-bind="attrs" v-on="on" class="buton1" >
             Fiyat
            </div>
            </template>
            <v-list class="kategorilist" >
             <div :class="{ red20 : gecersiz20 }" @mouseover="kirmizi20" @mouseleave="gecersiz20=false">1,000,000TL-1,498,000TL</div>
             <div :class="{ red21 : gecersiz21 }" @mouseover="kirmizi21" @mouseleave="gecersiz21=false">1,500,000TL-1,998,000TL</div>
             <div :class="{ red22 : gecersiz22 }" @mouseover="kirmizi22" @mouseleave="gecersiz22=false">2,000,000TL-2,498,000TL</div>
            </v-list>
         </v-menu>
        </v-row>
      </v-col>
      <v-col>
        <v-row>
          <v-menu  open-on-hover offset-y  >
           <template v-slot:activator="{ on, attrs }">
            <div v-bind="attrs" v-on="on" class="buton1">
             Renk
            </div>
            </template>
             <v-list class="kategorilist" >
             <v-radio :class="{ red23 : gecersiz23 }" @mouseover="kirmizi23" @mouseleave="gecersiz23=false" label="Metalik Gri"></v-radio>
             <v-radio :class="{ red24 : gecersiz24 }" @mouseover="kirmizi24" @mouseleave="gecersiz24=false" label="Rose Gold"></v-radio>
             <v-radio :class="{ red25 : gecersiz25 }" @mouseover="kirmizi25" @mouseleave="gecersiz25=false" label="Siyah"></v-radio>
             <v-radio :class="{ red26 : gecersiz26}" @mouseover="kirmizi26" @mouseleave="gecersiz26=false" label="Kahverengi"></v-radio>
             <v-radio :class="{ red27 : gecersiz27}" @mouseover="kirmizi27" @mouseleave="gecersiz27=false" label="Beyaz"></v-radio>
             <v-radio :class="{ red28 : gecersiz28 }" @mouseover="kirmizi28" @mouseleave="gecersiz28=false" label="Pempe"></v-radio>
            </v-list>
         </v-menu>
        </v-row>
      </v-col>
      <v-col>
        <v-row>
          <v-menu  open-on-hover offset-y  >
           <template v-slot:activator="{ on, attrs }">
            <div v-bind="attrs" v-on="on" class="buton1">
             Kayış Tipi
            </div>
            </template>
             <v-list class="kategorilist" >
              <v-radio :class="{ red29 : gecersiz29 }" @mouseover="kirmizi29" @mouseleave="gecersiz29=false" label="Çelik"></v-radio>
              <v-radio :class="{ red30 : gecersiz30}" @mouseover="kirmizi30" @mouseleave="gecersiz30=false" label="Deri"></v-radio>
            </v-list>
         </v-menu>
        </v-row>
      </v-col>
      <v-col>
        <v-row>
          <v-menu  open-on-hover offset-y  >
           <template v-slot:activator="{ on, attrs }">
            <div v-bind="attrs" v-on="on" class="buton1">
             Tarz
            </div>
            </template>
             <v-list class="kategorilist" >
              <v-radio :class="{ red31: gecersiz31 }" @mouseover="kirmizi31" @mouseleave="gecersiz31=false" label="Spor Saatler"></v-radio>
              <v-radio :class="{ red32 : gecersiz32 }" @mouseover="kirmizi32" @mouseleave="gecersiz32=false" label="Klasik Saatler"></v-radio>
            </v-list>
         </v-menu>
        </v-row>
      </v-col>
      <v-col>
        <v-row>
          <v-menu  open-on-hover offset-y  >
           <template v-slot:activator="{ on, attrs }">
            <div v-bind="attrs" v-on="on" class="buton1">
             Teknoloji
            </div>
            </template>
             <v-list class="kategorilist" >
              <v-radio :class="{ red33 : gecersiz33 }" @mouseover="kirmizi33" @mouseleave="gecersiz33=false" label="Quartz"></v-radio>
              <v-radio :class="{ red34 : gecersiz34 }" @mouseover="kirmizi34" @mouseleave="gecersiz34=false" label="Otomatik"></v-radio>
            </v-list>
         </v-menu>
        </v-row>
      </v-col>
      <v-col class="buton1">Urun</v-col>
      <v-col class="buton1"></v-col>
      <v-col class="buton1"></v-col>
      <v-col class="buton1"></v-col>
      <v-col class="buton1"></v-col>
      <v-col class="buton1"></v-col>
      <v-col class="buton1"></v-col>
      <v-col>
        <v-row>
          <v-menu  open-on-hover offset-y  >
           <template v-slot:activator="{ on, attrs }">
            <div v-bind="attrs" v-on="on" class="buton1">
             Sıralama
            </div>
            </template>
             <v-list class="kategorilist" >
              <v-radio :class="{ red33 : gecersiz33 }" @mouseover="kirmizi33" @mouseleave="gecersiz33=false" label="Seçtiklerimiz"></v-radio>
              <v-radio :class="{ red34 : gecersiz34 }" @mouseover="kirmizi34" @mouseleave="gecersiz34=false" label="Fiyat Artan"></v-radio>
              <v-radio :class="{ red35 : gecersiz35 }" @mouseover="kirmizi35" @mouseleave="gecersiz35=false" label="Fiyat Azalan"></v-radio>
              <v-radio :class="{ red36 : gecersiz36 }" @mouseover="kirmizi36" @mouseleave="gecersiz36=false" label="Yeni Gelenler"></v-radio>
              <v-radio :class="{ red37 : gecersiz37 }" @mouseover="kirmizi37" @mouseleave="gecersiz37=false" label="İndirimler"></v-radio>
            </v-list>
         </v-menu>
        </v-row>
      </v-col>
      <v-col class="buton1"></v-col>
    </v-row>
  </v-container>
</div>
</template>

<script>
export default {
 data: () => ({
    gecersiz14: false,
    gecersiz15: false,
    gecersiz16: false,
    gecersiz17: false,
    gecersiz18: false,
    gecersiz19: false,
    gecersiz20: false,
    gecersiz21: false,
    gecersiz22: false,
    gecersiz23: false,
    gecersiz24: false,
    gecersiz25: false,
    gecersiz26: false,
    gecersiz27: false,
    gecersiz28: false,
    gecersiz29: false,
    gecersiz30: false,
    gecersiz31: false,
    gecersiz32: false,
    gecersiz33: false,
    gecersiz34: false,
    gecersiz35: false,
    gecersiz36: false,
    gecersiz37: false,
    gecersiz38: false,
  }),

  methods:{
  kirmizi14() {
      this.gecersiz14 = true;
  },
  kirmizi15() {
      this.gecersiz15 = true;
  },
  kirmizi16() {
      this.gecersiz16 = true;
  },
  kirmizi17() {
      this.gecersiz17 = true;
  },
  kirmizi18() {
      this.gecersiz18 = true;
  },
   kirmizi19() {
      this.gecersiz19 = true;
  },
   kirmizi20() {
      this.gecersiz20= true;
  },
  kirmizi21() {
      this.gecersiz21= true;
  },
  kirmizi22() {
      this.gecersiz22= true;
  },
   kirmizi23() {
      this.gecersiz23= true;
  },
   kirmizi24() {
      this.gecersiz24= true;
  },
   kirmizi25() {
      this.gecersiz25= true;
  },
   kirmizi26() {
      this.gecersiz26= true;
  },
   kirmizi27() {
      this.gecersiz27= true;
  },
   kirmizi28() {
      this.gecersiz28= true;
  },
    kirmizi29() {
      this.gecersiz29 = true;
  },
   kirmizi30() {
      this.gecersiz30= true;
  },
  kirmizi31() {
      this.gecersiz31= true;
  },
  kirmizi32() {
      this.gecersiz32= true;
  },
   kirmizi33() {
      this.gecersiz33= true;
  },
   kirmizi34() {
      this.gecersiz34= true;
  },
   kirmizi35() {
      this.gecersiz35= true;
  },
   kirmizi36() {
      this.gecersiz36= true;
  },
   kirmizi37() {
      this.gecersiz37= true;
  },
   kirmizi38() {
      this.gecersiz38= true;
  },
}
}
</script>

<style>
.satirbir{
  background: #F9F9F9;
  height: 45px;
  max-height: 45px;
}
.buton1{
  background: #F9F9F9;
  max-width: 100px;
  height:20px;
  white-space: nowrap;
  color: #353535;
  font-size: 16px;
  min-height:0px
}
.red14 {
  background: gray;
  color: black;
}
.red15 {
  background: gray;
  color: black;
}
.red16 {
  background: gray;
  color: black;
}
.red17 {
  background: gray;
  color: black;
}
.red18 {
  background: gray;
  color: black;
}
.red19{
  background: gray;
  color: black;
}
.red20 {
  background: gray;
  color: black;
}
.red21 {
  background: gray;
  color: black;
}
.red22 {
  background: gray;
  color: black;
}
.red23 {
  background: gray;
  color: black;
}
.red24 {
  background: gray;
  color: black;
}
.red25 {
  background: gray;
  color: black;
}
.red26 {
  background: gray;
  color: black;
}
.red27 {
  background: gray;
  color: black;
}
.red28 {
  background: gray;
  color: black;
}
.red29 {
  background: gray;
  color: black;
}
.red30 {
  background: gray;
  color: black;
}
.red31 {
  background: gray;
  color: black;
}
.red32 {
  background: gray;
  color: black;
}
.red33 {
  background: gray;
  color: black;
}
.red34 {
  background: gray;
  color: black;
}
.red35 {
  background: gray;
  color: black;
}
.red36 {
  background: gray;
  color: black;
}
.red37 {
  background: gray;
  color: black;
}
.red38 {
  background: gray;
  color: black;
}
.buton1:hover{
  background: white;
  color: #BD1818;
}
</style>