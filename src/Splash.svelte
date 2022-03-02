<script>
    
// TODO:
// sketch 'about' cards X
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

    <div class='about'>

        <div class='about-card reduce-card'>
            <div class='card-copy'>
                <h2>reduce</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
            </div>
            <img src='' alt=''>
        </div>

        <div class='about-card reuse-card'>
            <div class='card-copy'>
                <h2>reuse</h2>
                <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
            </div>
            <img src='' alt=''>
        </div>

        <div class='about-card replenish-card'>
            <div class='card-copy'>
                <h2>replenish</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
            </div>
            <img src ='' alt=''>
        </div>

    </div>

    <div class='image-break'>
    </div>

</main>

<style>
    .header {
        height: 100vh;
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 4rem;
    }
    .about-card {
        border: 1px solid red;
        margin: 4rem 0;
        padding: 1rem;
        height: 50vh;
        display: flex;
    }
    .about-card img {
        height: 100%;
        aspect-ratio: 1/1;
        background: pink;
    }
    .reuse-card {
        flex-direction: row-reverse;
        text-align: right;
    }
    .image-break {
        height: 100vh;
        width: 100%;
        background-image: url('../static/images/image-break-placheolder.jpg');
        background-size: cover;
        background-position: center;
        background-attachment: fixed;
        box-shadow: 
            inset 0 1rem 2rem rgb(0 0 0 / .05),
            inset 0 -1rem 2rem rgb(0 0 0 / .05);
    }
</style>