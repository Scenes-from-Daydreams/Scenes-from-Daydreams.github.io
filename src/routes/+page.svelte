<script>
    import topVideo from "$lib/topVideo.mp4";
</script>

<body>

    <video autoplay muted loop id="topVideo">
        <source src={topVideo} type="video/mp4">
    </video>

    <div class="topContent">
        <div class="navBar">
            <nav>
                <a href="/packages">portrait packages</a>
                <a href="/prints">prints</a>
                <a href="/blog">blog</a>
                <a href="/contact">contact</a>
            </nav>
        </div>
        <div class="titleBar">
            <p>scenes from daydreams</p>
        </div>
    </div>

    <div class="centerTitle">
        <h2>scenes from daydreams</h2>
        <h3>photography by maggie blake</h3>
    </div>

    <hr>

</body>

<style>

    body {
        background: #232323;
    }

    /* adapted from https://www.w3schools.com/howto/howto_css_fullscreen_video.asp */
    #topVideo {
        position: fixed;
        right: 0;
        bottom: 0;
        margin-bottom: -700px;
        min-width: 100%;
        min-height: 100%;
        opacity: 50%;
    }

    .topContent {
        width: 100%;
        background: rgba(0, 0, 0, 0.2);
    }


    .navBar {
        position: fixed;
        top: 0;
        padding-top: 1.75%;
        color: #ffffff;
        width: 30%;
    }

    .titleBar {
        position: fixed;
        top: 0;
        right: 0%;
        text-align: center;
        color: #ffffff;
        width: 100%;
    }

    a, a:hover, a:focus, a:active {
        text-decoration: none;
        font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 350;
        color: #ffffff;
        padding-left: 5px;
        padding-right: 5px;
    }

    p {
        position: relative;
        right: 0;
        /* top: -21px; */
        text-decoration: none;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 500;
        color: #ffffff;
        font-size: 20px;
    }

    .centerTitle {
        width: 25%;
        padding-left: 37.5%;
        padding-top: 7.5%;
        position: relative;
        text-align: center;

        font-size: 32px;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 100;

        color: #ffffff;
    }

    /* h2 {

    } */

    h3 {
        padding-bottom: 10%;
        
        font-size: 16px;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 100;
    }

    hr {
        position: relative;
        width: 10%;
        color: #ffffff;
    }
</style>