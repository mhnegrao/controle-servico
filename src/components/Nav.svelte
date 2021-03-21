<script>
  export let segment;
</script>

<!-- <style> 
	nav {
		border-bottom: 1px solid rgba(255,62,0,0.1);
		font-weight: 300;
		padding: 0 1em;
	}

	ul {
		margin: 0;
		padding: 0;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
	}

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: rgb(255,62,0);
		display: block;
		bottom: -1px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
	}
</!-->
<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
	<div class="container-fluid">
	  <a class="navbar-brand" href=".">Navbar</a>
	  <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
		<span class="navbar-toggler-icon"></span>
	  </button>
	  <div class="collapse navbar-collapse" id="navbarNav">
		<ul class="navbar-nav">
			<li class="nav-item"><a class="nav-link" aria-current="{segment === undefined ? 'page' : undefined}" href=".">Home</a></li>
			<li class="nav-item"><a class="nav-link" aria-current="{segment === 'usuarios' ? 'page' : undefined}" href="usuarios">Usuários</a></li>
			<li class="nav-item"><a class="nav-link" aria-current="{segment === 'clientes' ? 'page' : undefined}" href="clientes">Clientes</a></li>
			<li class="nav-item"><a class="nav-link" aria-current="{segment === 'servicos' ? 'page' : undefined}" href="servicos">Serviços</a></li>
			<li class="nav-item"><a class="nav-link" aria-current="{segment === 'about' ? 'page' : undefined}" href="about">Sobre</a></li>
		</ul>
	  </div>
	</div>
  </nav>
