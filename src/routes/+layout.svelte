<div class="navBar">
    <a href="/packages">portrait packages</a>
    <a href="/blog">blog</a>
    <a href="/contact">contact</a>
    <div class="navBar-center">
        <a href="/test">scenes from daydreams</a>
    </div>
</div>

<slot>
</slot>

<style>
        /* navBar help from https://www.w3schools.com/howto/tryit.asp?filename=tryhow_css_topnav_centered */
    .navBar {
        position: fixed;
        top: 1%;
        width: 100%;
        z-index: 1;
    }

    .navBar a, a:hover, a:focus, a:active {
        float: left;
        text-align: center;
        text-decoration: none;
        color: #ffffff;

        font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 350;
        padding-left: 5px;
        padding-right: 5px;
    }

    .navBar-center a {
        float: none;
        position: fixed;

        top: 3%;
        left: 50%;
        transform: translate(-50%, -50%);

        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 500;
        font-size: 20px;
    }
</style>