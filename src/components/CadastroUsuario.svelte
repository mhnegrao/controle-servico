<div class='container'>

<form on:submit={(event)=>{event.preventDefault();}}>
    <div class="form-group">
        <label for="nome">Nome</label>
        <input type="text" class="form-control" id="nome" name="nome" placeholder="Digite seu nome" />
    </div>
    <div class="form-group">
        <label for="email">Email</label>
        <input type="email" class="form-control" id="email" name="email" aria-describedby="emailHelp"
            placeholder="Digite seu email" />
    
    </div>
    <div class="form-group">
        <label for="password">Senha</label>
        <input type="password" class="form-control" id="password" name="password" placeholder="Senha" />
        <small id="emailHelp" class="form-text text-muted">Lembre-se de sua senha!</small>
    </div>
    <!-- <div class="form-check">
      <input type="checkbox" class="form-check-input" id="exampleCheck1" />
      <label class="form-check-label" for="exampleCheck1">Check me out</label>
    </div> -->
    <button type="submit" class="btn btn-primary">Salvar</button>
    <button type="reset" class="btn btn-dark">Limpar</button>
</form>
</div>