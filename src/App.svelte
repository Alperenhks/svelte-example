<script>
// @ts-nocheck

  import { Router, Route, Link } from 'svelte-routing';
  import Home from './routes/Home.svelte';
  import About from './routes/About.svelte';
</script>

<Router>
  <nav>
    <Link to="/">Home</Link>
    <Link to="about">About</Link>
  </nav>
  <Route path="/" component={Home} />
  <Route path="about" component={About} />
</Router>
