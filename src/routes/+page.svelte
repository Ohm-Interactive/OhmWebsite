<script>
    import "svelte/transition"
	import { fade } from "svelte/transition";
    let visible = false
    setTimeout(show, 1)
    function show(){
        visible = true;
    }
</script>
<div class="Main">
    {#if visible}
        <section id="Home">
            <img in:fade src="OhmLogo.png" alt="Ohm Logo" class="Logo">
            <h1 in:fade>Ohm Interactive</h1>
            <p in:fade>Welcome to our official site!</p>
            <p in:fade>This is mainly just here for background info about us and the games we have made.</p>
        </section>
        <section id="About">
            <h2 in:fade>About us</h2>
            <p in:fade>We are just a small group that make cool projects</p>
            <p in:fade>There are currently only 7 people in Ohm Interactive. They are:</p>
            <div in:fade class="Names">
                <div>
                    <h2 style="padding-left: 20px;">Twingamerdudes</h2>
                    <p style="padding-left: 20px;">Contact: twingamerdudes#1389 (Discord)</p>
                    <br>
                    <img src="Twingamerdudes.jpg" alt="Twingamerdude's logo">
                </div>
                <div>
                    <h2 style="padding-left: 20px;">Omega</h2>
                    <p style="padding-left: 20px;">Contact: OmegaaDev#2871 (Discord)</p>
                    <br>
                    <img src="Omega.jpg" alt="Omega's logo">
                </div>
                <div>
                    <h2 style="padding-left: 20px;">Inovade</h2>
                    <p style="padding-left: 20px;">Contact: inovade#4388 (Discord)</p>
                    <br>
                    <img src="Inovade.png" alt="Inovade's logo" class="LargeImage">
                </div>
                <div> 
                    <h2 style="padding-left: 20px;">"Big Poop"</h2>
                    <p style="padding-left: 20px;">Contact: Big poop#5376 (Discord)</p>
                    <br>
                    <img src="BigPoop.png" alt='"Big Poops" logo' class="LargeImage">
                </div>
                <div> 
                    <h2 style="padding-left: 20px;">Tob</h2>
                    <p style="padding-left: 20px;">Contact: Tob#1798 (Discord)</p>
                    <br>
                    <img src="Tob.png" alt="Tob's logo" class="LargeImage">
                </div>
                <div> 
                    <h2 style="padding-left: 20px;">Crow</h2>
                    <p style="padding-left: 20px;">Contact: crow#0173 (Discord)</p>
                    <br>
                    <img src="Crow.png" alt="Crow's logo" class="LargeImage">
                </div>
                <div> 
                    <h2 style="padding-left: 20px;">Kyojiwa</h2>
                    <p style="padding-left: 20px;">Contact: Kyojiwa#1710 (Discord)</p>
                    <br>
                    <img src="Kyojiwa.png" alt="Kyojiwa's logo" class="LargeImage">
                </div>
            </div>
        </section>
        <br>
        <section id="Games">
            <div in:fade class="Main">
                <h2>Games</h2>
                <p>None at the moment :(</p>
                <p>Were working on it.</p>
            </div>
        </section>
        <br>
        <section id="Contact">
            <h2>Contact</h2>
            <p>Email: ohminteractiveofficial@gmail.com</p>
        </section>
    {/if}
</div>
<style lang="scss">
    .Logo{
        height: 20%;
        width: 20%;
    }
    .Main{
        display: flex;
        align-items: center;
        text-align: center;
        flex-direction: column;
    }
    @media only screen and (max-width: 1000px){
        .Names{
            flex-direction:column;
        }
    }
    .Names{
        display: flex;
        align-items: center;
        text-align: center;
    }
    h1,
    h2,
    p{
        margin-bottom: 1px;
    }
    .LargeImage{
        margin-left: 20px;
        height: 176px;
        width: 176px;
    }
</style>