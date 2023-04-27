<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
 
    <header>
    <img alt="Vue logo" class="logo" src="@/assets/vuejs.png" width="500" height="200" />   
  </header>
  <br>
  <div class="wrapper">
      <HelloWorld msg="this is our production.!" />
      <h2>You can rest assured that our experienced team can do everythings on the website and app according to the customer's needs with efficiency and high quality.</h2>

     <h1>
      <nav>
        <RouterLink to="/">tool for dev</RouterLink>
        <RouterLink to="/about">Go to our works</RouterLink>
      </nav>
     </h1>
      <h3>ຖ້າຫາກວ່າທ່ານມີຄວາມຕ້ອງການໜ້າເວັບໄຊຫຼືເອັບທີ່ເໝາະກັບການໃຊ້ງານຮ້ານຫຼືໜ້າວຽກຂອງທ່ານ, ທ່ານສາມາດຕິດຕໍ່ໄດ້ຈາກທິມງານ ອີໂກ ຂອງພວກເຮົາ. 
        ທີມງານຂອງພວກເຮົາຍິນດີພ້ອມໃຫ້ຄຳປືກສາແລະຊ່ວຍທ່ານໄດ້ຈາກລາຄາເລີ່ມຕົ້ນພຽງແຕ່ $200 ຮັບປະກັນຄວາມປອດໄພແລະໄວ້ວ່າງໃຈໄດ້.
      </h3>
    </div>
    

  <RouterView />
  
  
</template>

<style scoped>
body {
  background-color: aliceblue;
}

header {
  line-height: 1.5;
  max-height: 100vh;
  margin-top: 10px;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 200%;
  font-size: 20px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
