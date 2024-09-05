<script>
    import topVideo from "$lib/topVideo.mp4";
</script>

<body>

    <ol>
        <li id="screenOne">
            <div class="videoContainer">
                <video autoplay muted loop id="topVideo">
                    <source src={topVideo} type="video/mp4">
                </video>
            </div>
    
            <div class="centerTitle">
                <h2>scenes from daydreams</h2>
                <h3>photography by maggie blake</h3>
                <hr>
            </div>


        </li>

        <li id="screenTwo">

        </li>
    </ol>

</body>

 <style>

    :global(body) {
        margin: 0;
        padding: 0;
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
    }

    li {
        display: block;
        position: relative;
        width: 100%;
        height: 100vh;
        float: left;
        margin: 0;
        padding: 0;      
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
        position: absolute;
        left: 37.5%;
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
        width: 35%;
        color: #ffffff;
    }

    #screenTwo {
        background: #232323;
    }

</style>
