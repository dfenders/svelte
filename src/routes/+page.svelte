<!-- CSS - styling -->
<style>
    :root{
        --color:red;
    }
    h1{
        color:var(--color);
        font-size:34px;
        font-style: italic;
        font-weight: normal;
    }
    div{
        background:var(--color);
    }
</style>

<!-- JS - functionality -->
<script>    

    let colours = [
        "red",
        1,
        true,
        false,
        [1,2,3],
        "blue",
        "green"
    ];

    colours.forEach(x => {
        console.log(x);
    })
    
    let first_name = "Adosdfsdfn";
    let last_name = "Moskal";

    let writeName = () =>
    {
        return `${first_name} ${last_name}`;
    }

    let count = 0;

    let incrementCount = () => {
        count++;
    }

    let randomColour;

    function changeColour(){
        let r = Math.floor(Math.random() * 255);
        let g = Math.floor(Math.random() * 255);
        let b = Math.floor(Math.random() * 255);
      
        randomColour = `rgb(${r},${g},${b})`;
    }
    
</script>

<h1>{first_name}</h1>
<!-- HTML - structure -->
<button on:click={changeColour} style="background:{randomColour}">
    Clicked {count} {count === 1 ? 'time' : 'times'}
</button>
<div>
    {writeName()}
</div>