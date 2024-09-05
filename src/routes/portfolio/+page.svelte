<script>
// @ts-nocheck
    // const imageModules = import.meta.glob(
    //     '$lib/images/*.{jpeg,jpg}',
    //     {
    //         eager: true,
    //         query: {
    //             enhanced: true
    //         }
    //     }
    // )

    const photoRange = Array.from({length: 42}, (x, i) => './src/lib/images/'+(i+1)+".jpg") // [1,2,3,4,5,6,7,8,9,10]

    // $: console.log(photoRange);
    // // $: console.log(imageModules) 
    
    const srcs= [];
    let r = 0;
    let c = 0;
    srcs[r] = [];
    
    photoRange.forEach((path) => {
         if (c == 3) {
             r++;
             srcs[r] = [];
             c = 0;
         }
         srcs[r][c] = path;
         c++;
    });

    // Object.entries(imageModules) as [_path , module]
        
    // export let data;

</script>

<div class="portfolio">
    <!-- <div class="folders">
        <a href="/portfolio/fashion">fashion</a>
        <a href="/portfolio/lifestyle">lifestyle</a>
    </div> -->

    <!-- <table>
        {#each srcs as row}
            <tr>
                {#each row as imgSrc}
                    <img src={imgSrc} alt="Portfolio"/>
                {/each}
            </tr>
        {/each}
    </table> -->

    <!-- {#each Object.entries(imageModules) as [_path, module]}
	    <enhanced:img src={module.default} alt="some alt text" />
        <p>{module.default}</p>
    {/each} -->

    <!-- <img src="./src/lib/images/1.jpg" alt="test"/> -->

    <!-- <img src="$lib/images/1.jpg" alt="test"/> -->

    <table> {#each srcs as row}

        <tr> {#each row as path}
    
            <td><img src="{path}" alt="test" /></td>

        {/each} </tr>

    {/each} </table>

    <!-- {#each photoRange as photoSrc}
        <img src="{srcs[0][0]}" alt="test"/>
        <p>{photoSrc}</p>
    {/each} -->

</div>

<style>

    :global(body) {
        margin: 0;
        padding: 0;
    }

    .portfolio {
        background: #232323;
        width: 100%;
        height: 100vh;
    }

    img {
        width: 75%;
        height: auto;
    }

    /* .folders {
        position: absolute;
        top: 5%;
        left: 46%;
    }

    a, a:hover, a:focus, a:active {
        float: left;
        text-align: center;
        text-decoration: none;
        color: #ffffff;

        font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 350;
        padding-left: 5px;
        padding-right: 5px;
    } */
</style>