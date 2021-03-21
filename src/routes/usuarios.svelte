<script>
  import CadastroUsuario from "../components/CadastroUsuario.svelte";
  import ListaUsuarios from "../components/ListaUsuario.svelte";
  import { onMount } from "svelte";

const apiURL = "https://jsonplaceholder.typicode.com/todos";
let data = [];
  let isVisible = false;
  let usuarios = [];
  let usuario = {
    nome: "Marcelo",
    email: "marcelo@email.com",
    dataCadastro: Date.now(),
  };
  usuarios = usuarios.concat(usuario);

  const showFormulario = () => {
    isVisible = !isVisible;
  };
</script>

<section>
  <div class="container">
    <h3>Usuários</h3>
    <div class="row text-center">
      <button class="btn btn-primary" on:click={showFormulario}
        >Formulário de Cadastro</button
      >
    </div>
    {isVisible}
    <div class="row">
      {#if isVisible}
        <CadastroUsuario />
      {/if}
    </div>

    <div class="row">
      {#if usuarios && !isVisible}
        {#each usuarios as esteUsuario}
          <ListaUsuarios usuario={esteUsuario} />
        {/each}
      {/if}
    </div>
  </div>
</section>
