<script setup>
import { MaskedTextBoxComponent as EjsMaskedtextbox } from
       "@syncfusion/ej2-vue-inputs";
const customCharacters = {P: 'P,A,a,p',M: 'M,m'};

import {ref} from 'vue';

const value=ref(null);
</script>

<template>
 <div class="wrapper">
  <!-- <div className='label'>Mobile Number</div>  -->
  <ejs-maskedtextbox  floatLabelType='Auto'
 mask='[0-9][0-9][0-9][0-9]' placeholder='Enter pin code' v-model="value"
  ></ejs-maskedtextbox>
  <ejs-maskedtextbox v-model="value"
  ></ejs-maskedtextbox>
  </div>
</template>

<style scoped>
 @import "../node_modules/@syncfusion/ej2-base/styles/material.css";
@import "../node_modules/@syncfusion/ej2-inputs/styles/material.css";

 .wrapper{
  text-align: left;
  margin-bottom:150px;
  width: 240px;
}
.label{
  margin-bottom: 10px;
  font-weight: 600;
}
</style>
