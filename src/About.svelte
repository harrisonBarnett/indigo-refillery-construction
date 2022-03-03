<script>

</script>

<main>
    <div class='about'>
        <div class='about-card lazy reduce'>
            <div class='card-copy'>
                <h2>reduce</h2>
                <p>We want to help you make thoughtful decisions about the things you buy, so we chose to source our products from vendors who share our goal of reducing the amount of packaging material to the bare minimum. Let's work together to make our consumption a little less conspicuous.</p>
            </div>
            <img src='' alt=''>
        </div>

        <div class='about-card lazy reuse'>
            <div class='card-copy'>
                <h2>reuse</h2>
                <p>An oft-overlooked aspect of living sustainably is simply reusing items that may appear spent. Have you grown fond the soap pump that you've been using for the past month? Hold onto it! Your soap doesn't care what container it lives in, and neither should you. If you intend to start fresh, know that we can provide you with sustainably-sourced reusable containers.</p>
            </div>
            <img src='' alt=''>
        </div>

        <div class='about-card lazy replenish'>
            <div class='card-copy'>
                <h2>replenish</h2>
                <p>Feel good about the things that you bring into your home. Replenish your conscience by making sustainability a part of your day-to-day. We can even save you the drive, as we'll show up to your doorstep to deliver your refills using the reusable container of your choice.</p>
            </div>
            <img src ='' alt=''>
        </div>

    </div>
    <!-- Intersection Observer -->
    <script>
        // intersection observer 'lazily loads' the cards as they scroll into viewport
        const options = {
            threshold: .75
        }
        let cardObserver = new IntersectionObserver((entries, observer) => {
            entries.forEach(entry => {
                if(entry.isIntersecting) {
                    let lazyCard = entry.target
                    lazyCard.classList.remove('lazy')
                    lazyCard.classList.add('loaded')
                    paletteObserver.unobserve(lazyCard)
                }
            })
        }, options)

		const cards = document.querySelectorAll('.about-card')
        cards.forEach(card => {
            cardObserver.observe(card)
        })
    </script>
</main>

<style>
    .about {
        max-width: 800px;
        margin: 8rem auto;
        position: relative;
    }
    .about-card {
        border: 1px solid red;
        width: 75%;
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
    .reuse {
        margin-left: auto;
        flex-direction: row-reverse;
        text-align: right;
    }
    
</style>