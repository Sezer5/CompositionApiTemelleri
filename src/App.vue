<template>
    <div>
        <h2>Yaş : {{ yas }}</h2>
        <h2>Ad Soyad : {{ adSoyad }}</h2>
        <button @click="handleClick">Tıkla</button>
    </div>
</template>

<script>

export default {
  name: 'App',
  setup(){
    let adSoyad='Sezer Ünalmış';
    let yas='35';
    const handleClick = ()=>{
        console.log('Tıklandı');
    }
    return {
        adSoyad,yas,handleClick
    }
  }
}
</script>


