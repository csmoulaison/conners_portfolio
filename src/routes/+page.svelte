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
    margin: 12px 0;
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

    margin: 200px 0;
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
    margin: 12px 0;
}

ul {
    font-size: 20px;
    list-style-type: none;
    margin: 0;
    padding: 0;
}

li {
    border: 1px solid var(--background-off-lighter-color);

    padding: 16px;
    border-radius: 0;

    backdrop-filter: blur(4px);

    margin: 16px 0;

    max-height: 23px;
    overflow: hidden;

    transition: all 0.15s linear;
}

li:hover {
    max-height: 160px;

    border-style: solid;
    background-color: var(--background-off-color);

    cursor: default;
}

li div {
    display: grid;
    grid-template-columns: 1fr 24px;

}

li div img {
    transition: all 0.05s linear;
    opacity: 0.25;
}

li:hover div img {
    opacity: 0%;
    transform: translateY(24px);
}

.split-grid-3 {
    display: grid;
    width: 125ch;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: first-baseline;
    gap: 16px;

    height: 660px;
}

.split-grid-3 h2 {
    font-size: 26px;
    font-weight: bold;
    margin: 0;
}

.split-grid-2 {
    display: grid;
    width: 125ch;
    grid-template-columns: 1fr 1fr;
    align-items: first-baseline;
    gap: 48px;
}

.split-grid-2 h2 {
    margin-top: 16px;
    margin-bottom: 0;
    font-size: 26px;
    font-weight: bold;
}

.split-grid-2 h3 {
    padding: 48px 0;
    color: var(--body-mid-color);

    transition: all 0.25s;
}

.split-grid-2 h3:hover {
    padding: 56px 0;
    color: var(--body-main-color);
    cursor: default;
}

.left-arrow {
    display: inline-block;
    padding-right: 2px;

    transition: all 0.25s;
}

.split-grid-2 h3:hover .left-arrow {
    transform: translateX(-4px);

    transition: all 0.25s;
}

.split-grid-2 p {
    margin-top: 12px;
}

a {
    color: var(--body-mid-color);
    font-weight: bold;

    transition: all 0.15s linear;
}

a:hover {
    color: var(--body-main-color);
}

.arrow {
    display: inline-block;
    transform: translateX(2px);

    transition: all 0.1s linear;
}


a:hover .arrow {
    transform: translateX(6px);
}

.example-card {
    display: flex;
    flex-direction: column;
    gap: 8px;

    border: 3px solid var(--background-off-lighter-color);
    background-color: var(--background-off-color);
    padding: 0px;
    border-radius: 16px;

    overflow: hidden;
}

.example-card img {
    width: 100%;
    object-fit: cover;
}

.example-card p {
    margin: 0;
}

.example-header {
    margin-bottom: 24px;
}

.example-header span {
font-family: "Inter";
    color: var(--body-mid-color);
    font-size: 24px;
    font-weight: bold;
}

.example-selector {
    font-weight: bold;
    margin-bottom: 28px;
    display: flex;
    gap: 8px;
    color: var(--background-off-lighter-color);
}

.example-selector span {
    padding: 8px;
    transition: all 0.25s;
}

.example-selector span:hover {
    color: var(--body-mid-color);
    cursor: pointer;
}

.example-selector span.active {
    color: var(--body-mid-color);
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

footer {
    margin-bottom: 200px;
    display: flex;
    align-items: center;
    gap: 32px;
}

@media only screen and (max-width: 1020px) {
    main {
        margin: 0 12px;
    }

    .hello-conner {
        flex-direction: column;
        align-items: center;
        text-align: center;
        width: 100%;
    }

    .hello-conner p, .hello-conner h1 {
        animation-name: mobileslideup;
    }

    @keyframes mobileslideup {
        from {
            opacity: 0%;
            transform: translateY(16px);
        }
    }

    h1 {
        font-size: 40px;
    }

    h2 {
        margin: auto!important;
        text-align: center;
    }

    .split-grid-3 {
        width: 100%;
        grid-template-columns: 1fr;
        height: auto;
    }

    li {
        max-height: unset;
        border-style: solid;
    }

    footer {
        margin: 64px 0;
        flex-direction: column;
        gap: 32px;
    }

    footer div {
        display: none;
    }

    li div img {
        opacity: 0%;
    }
}

@media only screen and (max-width: 1400px) and (min-width:1021px) {
    .split-grid-3 {
        gap: 16px;
        width: 100ch;
    }

    .split-grid-3 h3 {
        font-size: 18px;
    }
}


</style>

<main>
    <div class='hello-conner'>
        <img src='me.jpg' height='225px'>
        <div>
            <h1>Hi, I'm Conner.</h1>
            <p>Self-taught game developer based in Ferndale, WA, United States</p>
        </div>
    </div>

    <div class='split-grid-3 slide-bottom'>
        <div>
            <h2>Who am I?</h2>
            <ul>
                <li>
                    <div>
                        <h3>System Administrator</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Oversaw the development of internal web applications and data integrations for the company</p>
                </li>

                <li>
                    <div>
                        <h3>Game Developer</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Self-taught designer/programmer and deeply interested in the relationship between algorithms and gameplay constructs</p>
                </li>

                <li>
                    <div>
                        <h3>Computer Enthusiast</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>I'm driven by curiosity about the way computers and software fundamentally work, both mechanically and philisophically</p>
                </li>

                <li>
                    <div>
                        <h3>Espresso Snob</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>If you must know, I'm currently loaded out with a Profitec GO and the Option-O Lagom Mini, and prefer light to medium roasts</p>
                </li>

                <li>
                    <div>
                        <h3>Lord of the Rings Guy</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>My favorite Vala is probably Ulmo, but I haven't thought about it in a while</p>
                </li>

                <li>
                    <div>
                        <h3>Modular Synth Programmer</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Well, I can dream, anyway</p>
                </li>
            </ul>
        </div>

        <div>
            <h2>What do I know?</h2>
            <ul>
                <li>
                    <div>
                        <h3>C/C++</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>I love low level programming, and have written in the C family for video games and other projects</p>
                </li>

                <li>
                    <div>
                        <h3>Assembly</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Dabbled in 16-bit ASM for an arcade game project, and can read x86 ASM to optimize code</p>
                </li>

                <li>
                    <div>
                        <h3>Python</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>I've found Python very useful for quick tooling, manipulating data to be used in game and work projects</p>
                </li>

                <li>
                    <div>
                        <h3>Excel</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Getting into Excel for quick management of data was a breakthrough for me both in work and personal projects. I'm handy with VBA, embarrasingly</p>
                </li>

                <li>
                    <div>
                        <h3>SQL</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>I use SQL almost every day in my System Administrator role to report on and manipulate business data</p>
                </li>

                <li>
                    <div>
                        <h3>Other</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>I've acquired a range of experience over the years, from SvelteKit web programming and Azure cloud services to exciting new niche languages like Odin</p>
                </li>
            </ul>
        </div>

        <div>
            <h2>What have I made?</h2>
                <li>
                    <div>
                        <h3>Crumble King (Arcade Game)</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Written in Odin (C-like language) using SDL 2 and Miniaudio</p>
                </li>

                <li>
                    <div>
                        <h3>Software Path Tracer</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Written in C and Win32 without math libraries, learning to use the profiler to effectively optimize code</p>
                </li>

                <li>
                    <div>
                        <h3>Vulkan Renderer</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Written in C++ and using SDL2 for windowing. Learned about GLSL and usage of fences and semaphores</p>
                </li>

                <li>
                    <div>
                        <h3>C Web Server</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Written in plain C and serves relatively simple HTML and CSS based on csv data for blog posts and the like</p>
                </li>

                <li>
                    <div>
                        <h3>Cicero (Language)</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>Compiled programming language written in C. So far I've written a simple lexer and LR parser and translated to NASM for the backend</p>
                </li>

                <li>
                    <div>
                        <h3>Other</h3>
                        <img src='arrow.svg'>
                    </div>
                    <p>CLI DM helper app for D&D in C#, unfinished Roguelike in C, practice projects in C/C++ such as Snake and Asteroids</p>
                </li>
        </div>

        
    </div>

    <footer>
        <a href="mailto:hello@connermoulaison.com">hello@connermoulaison.com</a>
        <div>/</div>
        <a href="tel:360-961-5549">360.961.5549</a>
        <div>/</div>
        <a href="/conner_moulaison_resume.pdf">see resume</a>
    </footer>
</main>
