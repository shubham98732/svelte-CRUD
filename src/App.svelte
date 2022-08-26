<script>
	import { Router, Link, Route } from "svelte-routing";
	import "../node_modules/materialize-css/dist/css/materialize.min.css";
  import "../node_modules/materialize-css/dist/js/materialize.min.js";
  import NavBar from './layout/NavBar.svelte';
  import Home from './pages/Home.svelte';
  import About from './pages/About.svelte';
	
</script>

<Router>
	<NavBar/>
	<div class='container'>
		<Route path="/" component={Home} />
		<Route path="/about" component={About} />
	</div>
</Router>

