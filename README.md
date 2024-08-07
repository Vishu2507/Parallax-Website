# Parallax-Website
Website With parallax effect
 # HTML
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="wrapper">
        <div class="container">
            <img src="background.png" class="background">
            <img src="foreground.png" class="foreground">
            <h1 style=" color:white">ADVENTURE</h1>

        </div>

        <section>
            <h2 class="secHeading">Adventure Time!</h2>
            <p class="text">
                Adventure is an exhilarating journey that pushes boundaries, tests courage, and creates unforgettable memories. It often involves exploring the unknown, facing challenges, and embracing the thrill of discovery. Whether through travel, outdoor activities, or new experiences, adventure enriches life with excitement and personal growth.

            <br> <br>
            Adventure is the pursuit of excitement and discovery, pushing limits, facing challenges, and creating lasting memories through thrilling experiences.
            </p>

            <div class="bg bg1">
                <h2 class="desc">BIKING</h2>
            </div>

                <p class="text">
                    Biking offers excitement and freedom, pushing physical limits, exploring new terrains, and creating lasting memories through exhilarating rides and scenic journeys.
                    <br> <br>
                    Biking combines physical endurance with the thrill of exploration, allowing riders to traverse diverse landscapes, discover new places, and experience a sense of freedom. It fosters health, adventure, and unforgettable memories.
                </p>

            <div class="bg bg2">
                <h2 class="desc">SURFING</h2>
            </div>

                <p class="text">
                    Surfing is an exhilarating sport that combines balance, skill, and the power of the ocean. Riding waves offers an unmatched thrill and connection to nature. It fosters a sense of freedom and adventure, creating unforgettable moments of gliding across water and mastering the art of wave riding.
                    <br><br>
                    Surfing involves riding waves with agility and balance, offering a thrilling connection to the ocean and fostering a deep sense of adventure.
                </p>

                <div class="bg bg3">
                    <h2 class="desc">PARA GLIDING</h2>
                </div>
    
                    <p class="text">
                        Paragliding offers an unparalleled sense of freedom and adventure, soaring high above landscapes with breathtaking views. It combines skill and courage, providing an adrenaline rush as you glide through the air. This thrilling sport allows for a unique connection to the sky and unforgettable aerial experiences.
                        <br><br>
                        Paragliding provides an exhilarating experience of flying, combining skill and bravery, allowing one to enjoy stunning aerial views and a unique freedom. 
                    </p>

        </section>

    </div>
</body>
</html>

# CSS 
*{
    padding: 0;
    box-sizing: border-box;
    margin: 0;
}

#wrapper{
    height:100vh;
    overflow-y: auto;
    overflow-x: hidden;
    perspective: 10px;
}

.container{
    position: relative;
    height:100%;
    transform-style: preserve-3d;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: -1;
}
.background{
    transform: translateZ(-35px) scale(5);
}
.foreground{
    transform: translateZ(-20px) scale(3);
}
.background, .foreground{
    position: absolute;
    height:100%;
    width:100%;
    object-fit: cover;
    z-index: -1;
}
h1{
    position:absolute;
    font-size: 8rem;
    color:white;
    top:5rem;
    letter-spacing: 4px;
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    text-shadow: 0 0 10px rgba(0,0,0,0.3);
    
}
section{
    background-color: rgb(45,45,45);
    color:white;
    padding:5rem 0;
}
.bg{
    background-attachment: fixed;
    position: relative;
    width: 100%;
    height:500px;
    background-size: cover;
    background-position: center;
}
.bg1{
    background-image: url(sport-1.jpg);
}
.bg2{
    background-image: url(sport-3.jpg);
}
.bg3{
    background-image: url(sport-2.jpg);
}
.secHeading{
    font-size: 5rem;
    padding:0 10rem;
}
.text{
    font-size:1.5rem;
    padding:0 10rem;
    margin: 4rem 0;
}
.desc{
    position:absolute;
    background-color: white;
    padding:0.5rem 2.5rem;
    top:40%;
    left:50%;
    color:black;
    font-size: 3.5rem;
    font-weight: 600;
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

    transform: translateX(-50%);
}
