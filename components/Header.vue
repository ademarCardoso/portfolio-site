<template>

  <div class="container-component">
    <img class="image-perfil" src="../static/asset-perfil-image.jpeg" alt="Imagem de perfil do Ademar Cardoso, desenvolvedor deste site.">

  <p class="name-perfil">
    Ademar Cardoso
    Front-end Developer 
  </p>

  <Bio />

  <div class="links-bio">
    <a href="https://github.com/teckthor" title="Link para a conta do github"><i class="fab fa-github"></i></a>
    <a href="http://#" title="Link para a conta do medium"><i class="fab fa-medium"></i></a>
    <a href="http://#" title="Link para a conta do instagram"><i class="fab fa-instagram"></i></a>
    <a href="http://#" title="Link para a conta do linkedin"><i class="fab fa-linkedin"></i></a>
  </div>

  </div>  
</template>

<script>
import Bio from './Bio'

export default {
  name: "Header",
  components: {
    Bio
  }
}
</script>

<style>
.container-component {
  /* max-width: 100% !important; */
  /* height: auto; */
  display: flex;
}

.image-perfil {
  display: flex;
  margin: 0 35px 0 35px;
  width: 20%;
  border-radius: 20px;
  margin-top: 45px; 
}

.name-perfil {
  font-size: 2.4em;
  font-weight: 700;
  text-align: center;
  display: flex;
  width: 100%;
  position: absolute;
  padding-top: 60px; 
  margin-left: 350px;
  height: 80px;
}

.links-bio {
  display: flex;
  flex-direction: column;
  margin-top: 110px;
  float: right;
  margin-left: 85px;
}

.links-bio a:not(:first-child) {
  padding-top: 15px;
}

a {
  margin-left: 20px;
  font-size: 2.3em;
  transition: all .2s;
}
a:hover{
  -moz-transform: scale(1.2);
	-webkit-transform: scale(1.2);
  transform: scale(1.2);
}

@keyframes blink {
  0%, 100% { opacity: 0; }
  50% { opacity: 1; }
}

</style>