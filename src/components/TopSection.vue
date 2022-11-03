<template>
        <header>
          <a class="main_link" href="#">TomiP.com</a>
        </header>

        <h1><span>Tomi P</span> Link Tree</h1>

        <div class="description">
          <p>
            A cappella Musician, Youtube Bass Singer and Front-End Developer
          </p>
        </div>
</template>

<script setup>

</script>

<style>
  .description{
      background-color: rgb(65, 65, 65);
  }

  header{
      padding: 1em 0 3em 0;
  }

  .main_link{
      color: white;
      text-decoration: none;
      font-weight: bold;
      font-size: 1.3rem;
  }


  h1{
      font-size: 2.5rem;
      margin: 2em 0 1.3em 0;
      color: white;
  }

  h1 span{
      text-transform: uppercase;
      display: block;
      font-size: 4rem;
      position: relative;
      z-index: 1;
  }

  h1 span::before{
      content: ' ';
      position: absolute;
      width: 3.6em;
      background: rgb(22, 166, 177);
      height: .445em;
      z-index: -1;
  }

  .description p {
      font-size: 1.3rem;
      font-weight: bold;
      margin: -1.5em 1em 3em;
      color: white;
  }
</style>