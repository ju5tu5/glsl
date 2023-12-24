<script>
    import { Canvas } from '@threlte/core'
    import Scene from './Scene.svelte'
</script>

<div>
  <Canvas>
    <Scene />
  </Canvas>
</div>

<svelte:head>
  <link rel="stylesheet" href="/style.css">
</svelte:head>

<header>
  <h1>GLSL</h1>
  <p>A place where i experiment with GLSL shaders...</p>
</header>

<main>
  <slot />
</main>

<footer>
  <p><span>&copy;</span> Copyleft, all wrongs reversed.</p>
</footer>

<style>
  div {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
  }

  span {
    display: inline-block;
    transform: rotate(180deg);
  }
  
</style>