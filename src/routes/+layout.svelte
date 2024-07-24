<style>

:root {
    --body-main-color: rgba(225, 225, 225, 1);
    --body-mid-color: rgba(150, 150, 150, 1);
    --unhovered-link-color: var(--body-mid-color);
    --background-color: rgba(18, 18, 18, 1);
    --background-off-color: rgba(25, 25, 25, 1);
    --background-off-lighter-color: rgba(60, 60, 60, 1);

    --body-main-color: rgba(220, 225, 210, 1);
    --body-mid-color: rgba(150, 155, 145, 1);
    --unhovered-link-color: var(--body-mid-color);
    --background-color: rgba(16, 20, 22, 1);
    --background-off-color: rgba(20, 24, 26, 1);
    --background-off-lighter-color: rgba(60, 60, 60, 1);

    color: var(--body-main-color);
    background-color: var(--background-color);
    font-family: "Inter", sans-serif;
    font-weight: normal;


}

:global(::selection) {
    background: var(--body-main-color);
    color: var(--background-color);
}

:global(::-moz-selection) {
    background: var(--body-main-color);
    color: var(--background-color);
}

:global(body, html) {
    margin: 0;
    padding: 0;
}

:global(body) {
    position: relative;
}

:global(.bg-img) {
    background-image: url("grain.png");
    background-size: tiled;
    background-position: center;
    mix-blend-mode: screen;
    position: absolute;
    height: 100%;
    width: 100%;
    z-index: -1;
    opacity: 0.15;
}

a {
    color: var(--unhovered-link-color);
    font-size: 16px;

    transition: all 0.25s;
}

a:hover {
    color: var(--body-main-color);
    cursor: pointer;
}

li:first-child a {
    color: var(--body-main-color);
    font-weight: bold;
    font-size: 16px;
}

ul {
    list-style-type: none;
    margin-top: 0;
    margin-bottom: 0;
    padding: 0;

    display: flex;
    justify-content:center;
    align-items: baseline;
    gap: 32px;
}

li {
    margin-top: 32px;
}

</style>

<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&family=Lora:ital,wght@0,400..700;1,400..700&display=swap" rel="stylesheet">
</head>

<div class='bg-img'></div>

<nav>
    <ul>
        <li><a>Conner Moulaison</a></li>
        <li><a>Work</a></li>
        <li><a>Blog</a></li>
        <li><a>Contact</a></li>
    </ul>
</nav>

<slot></slot>
