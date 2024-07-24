<style>


main {
    display: flex;
    flex-direction: column;
    align-items: center;

}

h1, h2, h3 {
    font-weight: normal;
    margin: 0;
}

h1, h2 {
    font-family: "Lora", serif;
}

h1 {
    font-size: 64px;
}

h2 {
    font-size: 48px;
    margin: 128px 0;
}

h3 {
    font-size: 20px;
    font-weight: bold;
}

.hello-conner {
    display: flex;
    align-items: last baseline;
    gap: 32px;
    width: 75ch;

    margin: 256px 0;
}

.hello-conner p {
    margin-top: 8px;
    margin-bottom: 0;
}

.hello-conner p, .hello-conner h1 {
    animation-duration: 1s;
    animation-name: helloconnertext;
}

@keyframes helloconnertext {
    from {
        opacity: 0%;
        transform: translateX(32px);
    }
}

.hello-conner img {
    margin-bottom: 0;
    border-radius: 16px;
    border-top-left-radius: 96px;
    border-bottom-right-radius: 0;

    box-shadow: 32px 32px 32px rgba(0, 0, 0, 0.25);

    animation-duration: 1s;
    animation-name: imgstart;
}

@keyframes imgstart {
    from {
        border-radius: 50%;
        border-top-left-radius: 0;
        opacity: 0%;
    }
}

p {
    font-size: 20px;
    margin: 8px 0;
}

ul {
    font-size: 20px;
    list-style-type: none;
    margin: 0;
    padding: 0;
}

li {
    border: 3px dashed var(--background-off-lighter-color);
    background-color: var(--background-off-color);

    backdrop-filter: blur(5px);
    -webkit-backdrop-filter: blur(5px);

    padding: 16px;
    border-radius: 16px;

    margin: 16px 0;
}

.split-grid-3 {
    display: grid;
    width: 125ch;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: first-baseline;
    gap: 64px;
}

.split-grid-2 {
    display: grid;
    width: 125ch;
    grid-template-columns: 1fr 1fr;
    align-items: first-baseline;
    gap: 64px;
}

.split-grid-3 h2 {
    font-size: 26px;
    font-weight: bold;
    margin: 0;
}

a {
    color: var(--body-main-color);
    font-weight: bold;
}

.arrow {
    display: inline-block;
    transform: translateX(2px);

    transition: all 0.25s;
}

a:hover .arrow {
    transform: translateX(6px);
}

.example-card {
    display: flex;
    flex-direction: column;
    gap: 8px;

    background-color: var(--background-off-color);
    padding: 16px;
    border-radius: 16px;
}

.example-card img {
    width: 100%;
    object-fit: cover;
    border-radius: 16px;
}

.example-card p {
    margin: 0;
}

.slide-bottom {
    animation-duration: 1.5s;
    animation-name: slidebottom;
}

@keyframes slidebottom {
    0%,
    25% {
        opacity: 0%;
        transform: translateY(32px);
    }
}

</style>

<main>
    <div class='hello-conner'>
        <img src='me.jpg' height='225px'>
        <div>
            <h1>Hi, I'm Conner.</h1>
            <p>Freelance software developer based in Bellingham, WA, United States. <a href='/work'>See example work<span class='arrow'>-></span></a></p>
        </div>
    </div>

    <div class='split-grid-3 slide-bottom'>
        <div>
            <h2>Who am I?</h2>
            <p>I have been programming personally for over a decade, and have worked professionally in an IT/developer role for over a year.</p>
            <p>These experiences have shaped me in the following ways:</p>
            <ul>
                <li>
                    <h3>System Administrator for Barlean's Organic Oils, LLC</h3>
                    <p>Oversaw the development of internal web applications and data integrations for the company.</p>
                </li>
                <li>
                    <h3>Web Development Enthusiast</h3>
                    <p>Functional, engaging design should help both businesses and customers, and developers have a responsibility to demonstrate excellence in their work.</p>
                </li>
                <li>
                    <h3>Hobbyist Game Developer</h3>
                    <p>My childhood passion is game development, and I've spent many years of my life doing it, programming games from scratch and learning how things work.</p>
                </li>
            </ul>
        </div>

        <div>
            <h2>How can I help you?</h2>
            <p>Experience in a lead business technology position has honed my ability to identify both design and process improvements in the way businesses use technology.</p>
            <p>Potential opportunites for me to help you or your business include:</p>
            <ul>
                <li>
                    <h3>Website development or improvements</h3>
                    <p>Including visual/UX design or brand new functionality. I can be productive regardless of the site's underlying technology.</p>
                </li>
                <li>
                    <h3>Process streamlining and automations</h3>
                    <p>Digging into business processes and finding ways to improve them, including ERP systems, reporting, and Excel.</p>
                </li>
                <li>
                    <h3>Data insight and integrations</h3>
                    <p>Get your company data where and when you need it, and connect related services together such as your ERP system and ecommerce site.</p>
                </li>
            </ul>
        </div>

        <div>
            <h2>What am I proficient in?</h2>
            <p>Gained experience with the following technologies both at work and at home:</p>
            <ul>
                <li>
                    <h3>Industry-standard web tech</h3>
                    <p>Such as Wordpress, React, Svelte, Next.js, AWS, and Azure.</p>
                </li>
                <li>
                    <h3>Shopify</h3>
                    <p>Ecommerce platform for businesses looking to sell product.</p>
                </li>
                <li>
                    <h3>Sage X3</h3>
                    <p>ERP system for managing company processes and data.</p>
                </li>
                <li>
                    <h3>Excel/VBA Extensions</h3>
                    <p>Excel and Visual Basic scripting can help quickly and cheaply drive improvement.</p>
                </li>
                <li>
                    <h3>SQL and Other Data Queries</h3>
                    <p>Data querying to efficiently build reports or gather ad-hoc insights.</p>
                </li>
            </ul>
        </div>
    </div>
    
    <h2 class='my-work'>My Work</h2>
    <div class='split-grid-2'>
        <div class='example-card'>
            <img src='portfolio.png' height='500px'>
        </div>

        <div>
            <h3>Artist Portfolio for Hannah Rants</h3>
            <p>A stunning design and insanely hot babe bring an air of intrigue to this cost effective site.</p>
        </div>
    </div>

    <h2 class='outro'><a href='/contact'>Contact me</a> directly for a consultation. Thanks for stopping by!</h2>
</main>
