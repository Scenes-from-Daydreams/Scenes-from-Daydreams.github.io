<script>
    import topVideo from "$lib/topVideo.mp4";
</script>

<body>

    <div class="screenOne">

        <video autoplay muted loop id="topVideo">
            <source src={topVideo} type="video/mp4">
        </video>

        <div class="navBar">
            <a href="/packages">portrait packages</a>
            <a href="/blog">blog</a>
            <a href="/contact">contact</a>
            <div class="navBar-center">
                <a href="/test">scenes from daydreams</a>
            </div>
        </div>

        <div class="centerTitle">
            <h2>scenes from daydreams</h2>
            <h3>photography by maggie blake</h3>
            <hr>
        </div>


    </div>

    <!-- <div class="screenTwo">

        <svg width=100% height=100%>
            <rect width=100% height=100%/>
        </svg>
    </div> -->

</body>

 <style>

    /* body {
        background: #232323;
    } */

    /* :global(body) {
        background-color: #232323;
    } */

    .screenOne {
        position: relative;
        /* background: #232323; */
        width: 100%;
        height: 100%;
        background: rgba(0,0,0,0);
    }

    /* navBar help from https://www.w3schools.com/howto/tryit.asp?filename=tryhow_css_topnav_centered */
    .navBar {
        position: relative;
        padding-top: 1.75%;
        width: 100%;
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
        position: absolute;

        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);

        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 500;
        font-size: 20px;
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
        
        opacity: 100%;
        filter: brightness(75%);
    }

    .centerTitle {
        width: 25%;
        height: 25%;
        /* padding-left: 37.5%;
        padding-top: 7.5%; */
        position: fixed;
        left: 37.5%;
        top: 37.5%;
        text-align: center;

        font-size: 32px;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 100;

        color: #ffffff;
    }

    h3 {
        padding-bottom: 15%;

        font-size: 16px;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 100;
    }

    hr {
        /* position: relative; */
        width: 35%;
        color: #ffffff;
    }

    /* .screenTwo {
        position: relative;
        padding-top: 100%;
        min-width: 100%;
        min-height: 100%
    } */
</style>