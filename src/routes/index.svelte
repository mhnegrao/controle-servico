<script>
  import Login from "./login.svelte";
  import successkid from "images/successkid.jpg";
</script>

<svelte:head>
  <title>Controle Adm</title>
</svelte:head>

<h1>Plataforma Controle de Serviços!</h1>

<figure>
  <img alt="Success Kid" src={successkid} />
  <figcaption>Have fun with Sapper!</figcaption>
</figure>

<style>
  h1,  figure{
    text-align: center;
    margin: 0 auto;
  }

  h1 {
    font-size: 2.8em;
    text-transform: capitalize;
    font-weight: 700;
    margin: 0 0 0.5em 0;
  }

  figure {
    margin: 0 0 1em 0;
  }

  img {
    width: 100%;
    max-width: 400px;
    margin: 0 0 1em 0;
  }

  
  @media (min-width: 480px) {
    h1 {
      font-size: 4em;
    }
  }
</style>
