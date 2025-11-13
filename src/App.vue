<template>
    <div>
        <h2>Yaş : {{ yas }}</h2>
        <h2 ref="myRef">Ad Soyad : {{ adSoyad }}</h2>
        <button @click="handleClick">Tıkla</button>
    </div>
</template>

<script>
import {ref} from 'vue'
export default {
  name: 'App',
  setup(){
    let adSoyad='Sezer Ünalmış';
    let yas='35';
    const myRef=ref(null);
    const handleClick = ()=>{
        console.log(myRef,myRef.value);
        myRef.value.classList.add('can');
        myRef.value.textContent='Sezer';

    }
    return {
        adSoyad,yas,handleClick,myRef
    }
  }
}
</script>


