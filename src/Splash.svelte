<script>
    import About from './About.svelte'
    
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
        <h2>Purveyor of Mobile Sustainable Consumables</h2>

        <img class='header-img' src="../static/images/logo-outline.png" alt="a line illustration of an indigo flower">
        <p>Greenville, SC</p>
    </div>

    <About />

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
        gap: 2rem;
    }
    .header p {
        position: relative;
    }
    .header p::before, .header p::after {
        content: '';
        position: absolute;
        height: 1px;
        width: 50%;
        background: black;
        top: 50%;
    }
    .header p::before {
        right: 110%;
    }
    .header p::after {
        left: 110%;
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