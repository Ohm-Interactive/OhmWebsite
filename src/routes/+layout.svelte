<script>
    import "../app.css"
    import "../lib/Navbar.svelte"
	import Navbar from "../lib/Navbar.svelte";
</script>
<div class="Navbar">
    <Navbar></Navbar>
</div>
<main style="margin-top:120px">
	<slot />
</main>
<style>
    .Navbar{
        margin-bottom: 20px;
        background-color: #081d30;
        z-index: 99;
        top: 0;
        right: 0;
        left:0;
        position: fixed;
    }
</style>