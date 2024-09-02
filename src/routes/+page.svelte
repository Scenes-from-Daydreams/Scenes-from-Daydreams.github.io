<script>
    import topVideo from "$lib/topVideo.mp4";
</script>

<body>

    <ol>
        <li>
            <div class="videoContainer">
                <video autoplay muted loop id="topVideo">
                    <source src={topVideo} type="video/mp4">
                </video>
            </div>
    
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


        </li>

        <li>

            <!-- <svg width=100% height=100%>
                <rect width=100% height=100%/>
            </svg> -->

        </li>
    </ol>

    <!-- <div class="screenOne">
 
    </div>

    <div class="screenTwo">

    </div> -->

</body>

 <style>

    /* body {
        background: #232323;
    } */

    :global(body) {
        margin: 0;
        padding: 0;
        /* background-color: #232323; */
    }

    ol {
        display: block;
        position: relative;
        width: 100%;
        height: auto;
        float: left;
        margin: 0;
        padding: 0;
        list-style-type: none;
        /* padding-left: 0;
        padding-top: 0; */
    }

    li {
        display: block;
        position: relative;
        width: 100%;
        height: 100vh;
        float: left;
        margin: 0;
        padding: 0;
        /* padding-left: 0;
        padding-top: 0; */
        
    }

    /* .screenOne {
        position: relative;
        width: 100%;
        height: 100vh;
        background: rgba(0,0,0,0);
    } */

    /* navBar help from https://www.w3schools.com/howto/tryit.asp?filename=tryhow_css_topnav_centered */
    .navBar {
        position: fixed;
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
        position: fixed;

        top: 6%;
        left: 50%;
        transform: translate(-50%, -50%);

        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: 500;
        font-size: 20px;
    }

    /* adapted from https://www.w3schools.com/howto/howto_css_fullscreen_video.asp */
    #topVideo {
        position: relative;
        right: 0;
        bottom: 0;
        margin-bottom: -700px;

        z-index: -1;
        width: auto;
        min-width: 100%;
        height: auto;
        
        opacity: 100%;
        filter: brightness(75%);
    }

    .videoContainer { 
        width: 100%;
        overflow: hidden;   
        max-height: 100vh;
        position: absolute;
        z-index: -1;
    }

    .centerTitle {
        width: 25%;
        height: 25%;
        /* padding-left: 37.5%;
        padding-top: 7.5%; */
        position: absolute;
        left: 37.5%;
        /* top: 100%; */
        padding-top: 12.5%;
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
/* 
    .screenTwo {
        position: relative;
        padding-top: 100%;
        min-width: 100%;
        min-height: 100%
    } */

</style>