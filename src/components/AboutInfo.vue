<template>
    <section class="bottom_text">
      <div class="collum">
        <h2>About Tomi</h2>
        <p>
          Since 2016 I've been producing music on Youtube. I started with simple
          a cappella covers and over time ventured into more complex styles. I
          started to distribute my music to other platforms and created my own
          Patreon page where number of very generous people supported me over
          time. Around a year of 2017 I found my first vocal band in Brno in
          which I'm still singing. 2021 Me and my three friends from Discord
          started the first internation "only bass" group called The Bass Gang.
          Mid-year 2022 I started to learn coding and webdevelopment on my own
          and decided to take the route of Front-End Developing. Incompassing
          programming languages like HTML, CSS, JavaScript and other respective
          frameworks.
        </p>
      </div>
    </section>

    <section class="bottom_picture">
      <div>
        <img
          class="bottom_picture2"
          src="/src/imgs/Tomi_picure.jpg"
          alt=""
        />
      </div>
    </section>
</template>

<script setup>
</script>

<style>
.collum{
    text-align: center;
    margin: 3em 1em;
}

h2{
    text-transform: uppercase;
    position: relative;
}

h2::before{
    content: ' ';
    position: absolute;
    width: 6.6em;
    background: rgb(22, 166, 177);
    height: .445em;
    z-index: -1;
}

p{
    line-height: var(--leading);
    color: black
}
.bottom_picture{
    width: 100%;
    margin: 0;
}

.bottom_picture img{
    max-width: 100%;
    height: auto;
}

.bottom_picture div{
    text-align: center;
}

@media (min-width: 667px) {
  .bg_container section{
      width: 65%;
      margin: auto;
  }
} 

@media (min-width: 1350px) {
  .bottom_text p{
    margin-left: 15em;
    margin-right: 15em;
  }
  .bg_container section{
        margin: auto;
     }
}


</style>