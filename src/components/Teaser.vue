<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
</script>

<template>
  <div class="bg">
    <img src="/src/assets/capa.png" class="logo" title="Mateus Porto" alt="Mateus Porto logo" />

    <div class="buttons">
      <a href="https://mateusporto.mercadoshops.com.br/" target="_blank" class="btn">Compre a camiseta</a>
      <a href="https://drive.google.com/drive/folders/1H48fCwOe1dWlMQaoDyjujeTofb3JANwm?usp=share_link" target="_blank" class="btn btn-transparent">Baixe as músicas</a>
    </div>

    <div class="platforms">
      <p>disponível em todas as plataformas</p>
      
      <div class="platforms-links">
        <a href="https://open.spotify.com/artist/4ObrU6FYKTDkoHHMcMQu7R?si=Wg4FsFD5Q7G2VUtX6_XqEA" target="_blank"><img src="/src/assets/spotify.png" title="Spotify" alt="Spotify logo" /></a>
        <a href="https://deezer.page.link/Dz6WBQQPpvkYuCx68" target="_blank"><img src="/src/assets/deezer.png" title="Deezer" alt="Deezer logo" /></a>
        <a href="https://youtube.com/channel/UCpNefuxWnHVLjpmJ80ciBlA" target="_blank"><img src="/src/assets/youtube.png" title="YouTube" alt="YouTube logo" /></a>
        <a href="" target="_blank"><img src="/src/assets/napster.png" title="Napster" alt="Napster logo" /></a>
        <a href="https://tidal.com/browse/artist/9163965" target="_blank"><img src="/src/assets/tidal.png" title="Tidal" alt="Tidal logo" /></a>
        <a href="https://music.apple.com/br/artist/mateus-porto/1292428804" target="_blank"><img src="/src/assets/apple.png" title="Apple Music" alt="Apple Music logo" /></a>
        <a href="" target="_blank"><img src="/src/assets/google.png" title="Googlr Play" alt="Google Play logo" /></a>
        <a href="https://music.amazon.com.br/artists/B07664NKDL/mateus-porto?marketplaceId=A2Q3Y263D00KWC&musicTerritory=BR&ref=dm_sh_nYo6DUmX91bc34C09giNZlgmh" target="_blank"><img src="/src/assets/amazon.png" title="Amazon Music" alt="Amazon Music logo" /></a>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.bg {
  background: url("src/assets/hero.png") no-repeat center center;
  background-size: cover;
  height: 100vh;

  @media(max-width: 765px) {
    height: 100%;
  }
}
.logo {
  margin-top: 100px;
  width: 520px;

  @media(max-width: 765px) {
    width: 320px;
  }
}
.buttons {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  margin-top: 20px;
}
.btn {
  border: 2px solid #FFFFFF;
  background: #FFFFFf;
  border-radius: 50px;
  padding: 9px 35px;
  margin: 0 10px;
  font-weight: bold;
  color: #000000;
  transition: all 0.5s ease;

  &:hover {
    opacity: .6;
  }
}
.btn-transparent {
  background: transparent;
  color: #FFFFFF;

  @media(max-width: 765px) {
    margin-top: 15px;
  }
}
.platforms {
  margin-top: 100px;

  @media(max-width: 765px) {
    margin-top: 50px;
    padding-bottom: 40px;
  }
}
.platforms p {
  color: #FFFFFF;
}
.platforms-links {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
.platforms-links a {
  margin: 0 12px;
}
.read-the-docs {
  color: #888;
}
</style>


