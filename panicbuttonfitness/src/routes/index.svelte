<script>
	import 'animate.css';
    
    function handleClick() {
        window.location.reload();
        window.open(url, '_blank');
        win.focus();
        
}
    // LIST OF THE MOTIVATIONAL URLS AND THE RANDOM URL REQUEST //
    let urls = ['https://i.redd.it/btuzlz1j29091.jpg', 'https://i.redd.it/cewpkth8r0091.jpg', 'https://i.redd.it/58zmkboulqa81.png',
     'https://i.redd.it/76a0rrjt8hv81.jpg', 'https://i.redd.it/qa79tah4ld281.png', 'https://i.redd.it/l6w6o2q0mccx.jpg', 'https://i.redd.it/ws87e29ohnm71.png',
      'https://i.redd.it/tndahj18a7j81.jpg', 'https://i.redd.it/jj55kt0lflc81.jpg', 'https://i.redd.it/zwwuylio95251.jpg',
      'https://www.youtube.com/watch?v=TU7Y6HiLXto', 'https://www.youtube.com/watch?v=UNQhuFL6CWg&t', 'https://i.redd.it/zwwuylio95251.jpg', 
      'https://pbs.twimg.com/media/EvvYJIYWEAApnni?format=jpg&name=large', 'https://pbs.twimg.com/media/FUatHC6WYAIvWKg?format=jpg&name=medium', 
      'https://pbs.twimg.com/media/FePEMZFaEAEk4i9?format=jpg&name=medium', 'https://i.redd.it/56wkrudn71o91.jpg', 'https://i.redd.it/hxeaxednp6r91.jpg', 
      'https://i.redd.it/3o1rzz1vybm91.jpg', 'https://i.redd.it/h7qw4odimqr91.jpg', 'https://i.redd.it/8qtwkehdd2p91.jpg', 'https://i.redd.it/nhswjdpj6on91.jpg',
       'https://i.redd.it/qcst03bct9n91.jpg', 'https://i.redd.it/9pgb15frszq91.jpg', 'https://i.redd.it/ljnd12tumap91.jpg', 
       'https://www.azquotes.com/picture-quotes/quote-in-the-midst-of-winter-i-found-there-was-within-me-an-invincible-summer-and-that-makes-albert-camus-47-22-23.jpg'];
    let url = urls[Math.floor(Math.random() * urls.length)];

</script>

<body>
    <div class="main-container">
        <h3>Not in the mood for a workout?</h3>
        <h4>Hit the button below and get a shot of potent daily motivation to get you going!</h4>
        <div class=" animate__animated animate__pulse animate__repeat-3">
        <button class="theButton" on:click|capture={handleClick}></button>
        </div>
    </div>
</body>


<!-- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -->
<!-- START OF STYLING -->
<style>
    html,body {
        height: 100%;
        background-color: #E9E4D4;

        margin: 0;
        overflow: hidden;
    }

    .main-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100vh;
        width: 100%;
    } 
        h3 {
            font-family: 'Bebas Neue', cursive;
            font-size: 5rem;
            color: rgb(122, 28, 28);
      
        } 
        h4 {
            font-family: 'Bebas Neue', cursive;
            font-size: 1.5rem;
            color: rgb(122, 28, 28);
        } 
     
    .theButton {
        cursor: pointer;
        background: #f00;
        width: 300px;
        height: 300px;
        border-radius: 50%;
        -webkit-box-shadow: 15px 10px 10px 5px rgba(0,0,0,0.46); 
        box-shadow: 15px 10px 10px 5px rgba(0,0,0,0.46);
    }



    @media screen and (max-width: 991px) {
        h3 {
            padding-top: 10vw;
            font-family: 'Bebas Neue', cursive;
            font-size: 3.5em;
            text-align: center;
           
      
        } 

        h4 {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 50%;
            text-justify: center;
            font-family: 'Bebas Neue', cursive;
            font-size: 2.5em;
            text-align: center;
            padding-bottom: 5vw;
        }
        
        .theButton {
        cursor: pointer;
        background: #f00;
        width: 25em;
        height: 25em;
        border-radius: 50%;
        -webkit-box-shadow: 15px 10px 10px 5px rgba(0,0,0,0.46); 
        box-shadow: 15px 10px 10px 5px rgba(0,0,0,0.46);
        margin-bottom: 10vw;
    }
}

    @media screen and (max-width: 767px) {
         h3 {
            font-family: 'Bebas Neue', cursive;
            font-size: 2.8em;
            text-justify: center;
            color:black;
            display: flex;
            flex-direction: row;
            align-items: center;
        } 

        h4 {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 50%;
            text-justify: center;
            font-family: 'Bebas Neue', cursive;
            font-size: 2.1em;
            text-align: center;
            padding-bottom: 10%;
        }
        
        .theButton {
        cursor: pointer;
        background: #f00;
        width: 15em;
        height: 15em;
        border-radius: 50%;
        -webkit-box-shadow: 15px 10px 10px 5px rgba(0,0,0,0.46); 
        box-shadow: 15px 10px 10px 5px rgba(0,0,0,0.46);
    }


    @media screen and (max-width: 479px) {
        h3 {
            font-family: 'Bebas Neue', cursive;
            font-size: 1.9rem;
            text-align: center;
      
        } 
        h4 {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 70%;
            text-justify: inter-cluster;
            font-family: 'Bebas Neue', cursive;
            font-size: 1.2em;
            text-align: center;
            padding-bottom: 30%;
        }
        
        .theButton {
        cursor: pointer;
        background: #f00;
        width: 15em;
        height: 15em;
        border-radius: 50%;
        -webkit-box-shadow: 15px 10px 10px 5px rgba(0,0,0,0.46); 
        box-shadow: 15px 10px 10px 5px rgba(0,0,0,0.46);
    }
}




}



</style>
<!-- END OF STYLING -->