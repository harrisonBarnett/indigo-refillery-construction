<script>
    
// TODO:
// style 'about' cards
// intersection observer to load them from the sides on scroll
// add social icons to header
// style footer

</script>

<main>
    <div class='header'>
        <h1>The Wild Indigo Refillery</h1>
        <img class='header-img' src="../static/images/logo-outline.png" alt="a line illustration of an indigo flower">
        <h2>A Sustainable Consumables Market</h2>
    </div>

    <div class='image-break'>
    </div>

    <div class='about'>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
        <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>

</main>

<style>
    .header {
        height: 100vh;
        width: 100vw;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 2rem;
    }
    .image-break {
        height: 100vh;
        width: 100vw;
        margin: 12rem 0;
        background-image: url('../static/images/image-break-placheolder.jpg');
        background-size: cover;
        background-position: center;
        box-shadow: 
            inset 0 1rem 2rem rgb(0 0 0 / .25),
            inset 0 -1rem 2rem rgb(0 0 0 / .25);
    }
    .about {
        background-color: palevioletred;
    }
</style>