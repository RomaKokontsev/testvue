<template>
  <div :id="$style.app">
    <ApartmentsList :items="apartments" />
  </div>
</template>

<script>
import ApartmentsList from "./components/apartment/ApartmentsList.vue";
import apartments from "./components/apartment/apartments";
export default {
  name: "App",
  components: {
    ApartmentsList,
  },
  data() {
    return {
      apartments,
      apartment: {
        id: "34234kjgbkhgh4543hkgh",
        title: "fdlgdfg gfdngsln fgnsldfng fgnsldfnglsfd gfdglksdkgn gfkdsngl",
        descr: "Bfkdjslk sfgjdg  fdnbgsdfjgnlfd g dfjlsgnjsdfng gfdjbgsjfd",
        price: 2032,
        rating: 4.5,
        location: {
          city: "Kyiv",
        },
        owner: {
          name: "Ellen",
          phone: "115-355-5663",
          email: "tracey.morar86@hotmail.com",
        },
      },
    };
  },
};
</script>

<style module>
#app {
  font-family: Montserrat, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
