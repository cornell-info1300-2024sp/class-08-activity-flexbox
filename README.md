# INFO 1300 > Spring 24 > Activity > Flex Box

- Set a max viewing area for wide screens and center the content area inside the browser:

    `body {
        max-width: 1000px; /*set max width of content area */
        margin: 0 auto; /* center the content area */
    }`

- Setup the `<header>` so that the `<h1>` and `<nav>` are side by side using a flexbox:

    `header {
        display: flex; /* flex container */
        flex-direction: row; /* side by side */
        align-items: center; /* center in container */
        gap: 40px; /* add spacing between elements */
    }`

- Setup the `<nav>` so the links are side by side using flexbox:

    `nav ul {
       display: flex; /* flex the nav links */
        flex-direction: row; /* side by side */
    }`

- Setup the Welcome and Events content areas so the the text content and the images are side by side:

    --  Setup a generic flex container for side by side content:

        `.columns {
            display: flex;
            flex-direction: row;
            gap: 24px;
        }`

    -- Setup a generic class to center flex items.

        `.columns-center {
            align-items: center;
        }`

    -- Setup a flex container in the HTML that then uses these generic classes:

          `<div class="columns columns-center ...">`
