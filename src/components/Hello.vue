<template>
  <div class="hello">
    <Logo></Logo>
    <Goindex></Goindex>
    <Nav></Nav>
    <Carousel></Carousel>
    <Card></Card>
    <Facebook></Facebook>
    <Footer></Footer>
  </div>
</template>

<script>
import Logo from '../page/Logo'
import Goindex from '../page/Goindex'
import Nav from '../page/Nav'
import Carousel from '../page/Carousel'
import Card from '../page/Card'
import Facebook from '../page/Facebook'
import Footer from '../page/Footer'

export default {
  components:{
    Logo,
    Goindex,
    Nav,
    Carousel,
    Card,
    Facebook,
    Footer
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
