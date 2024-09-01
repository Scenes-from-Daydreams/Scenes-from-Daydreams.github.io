<script>
    import topVideo from "$lib/topVideo.mp4";
</script>

<!-- <body> -->

    <video autoplay muted loop id="topVideo">
        <source src={topVideo} type="video/mp4">
    </video>

    <!-- <div class="topContent"> -->
        <div class="navBar">
            <nav>
                <a class="leftNav" href="/packages">portrait packages</a>
                <a class="leftNav" href="/blog">blog</a>
                <a class="leftNav" href="/contact">contact</a>
                <a class="titleBar" href="/">scenes from daydreams</a>
            </nav>
        </div>
    <!-- </div> -->

    <!-- Make screen one be the whole first screen, not just the title. Then you can organize things around that div and give it a background? -->
    <!-- <div class="screenOne">

        <div class="centerTitle">
            <h2>scenes from daydreams</h2>
            <h3>photography by maggie blake</h3>
        </div>

        <hr>
    </div> -->

    <!-- <div class="screenTwo">

        <svg width=100% height=100%>
            <rect width=100% height=100%/>
        </svg>
    </div> -->

<!-- </body> -->

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

        z-index: -1;
        min-width: 100%;
        min-height: 100%;
        /* max-width: 100%;
        max-height: 100%; */
        
        opacity: 50%;
    }

    .topContent {
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.2);
    }

    .navBar {
        position: fixed;
        top: 0;
        padding-top: 1.75%;
        color: #ffffff;
        width: 30%;
    }

    .leftNav {
        text-decoration: none;
        font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 350;
        color: #ffffff;
        padding-left: 5px;
        padding-right: 5px;
    }

    .titleBar {
        position: fixed;
        padding-right: 50%;
        padding-top: 1.75%;
        text-align: center;
        text-decoration: none;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 500;
        color: #ffffff;
        font-size: 20px;
        top: 0;
        right: 0%;
        color: #ffffff;
        width: 20%;
    } 

    /* a, a:hover, a:focus, a:active {
        text-decoration: none;
        font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 350;
        color: #ffffff;
        padding-left: 5px;
        padding-right: 5px;
    } */

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
        padding-bottom: 15%;

        font-size: 16px;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 100;
    }

    hr {
        position: relative;
        width: 10%;
        color: #ffffff;
    }

    .screenTwo {
        position: relative;
        padding-top: 100%;
        min-width: 100%;
        min-height: 100%
    }
</style>