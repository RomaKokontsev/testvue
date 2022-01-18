<template>
  <div :id="$style.app">
    <ApartmentsItem
      :descr="apartment.descr"
      :price="apartment.price"
      :rating="apartment.rating"
    />
  </div>
</template>

<script>
import ApartmentsItem from "./components/apartment/ApartmentsItem.vue";
export default {
  name: "App",
  components: {
    ApartmentsItem,
  },
  data() {
    return {
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
