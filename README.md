<!DOCTYPE html>

<html>

<head>

 <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <link rel="icon" href="IMG_9112.JPG">
    <title>Rupayon Chakrabarty</title>


     /* Base Styles */
body {
    margin: 0;
    padding: 0;
    font-family: 'Arial', sans-serif;
    color: white;
    overflow: hidden;
    height: 100vh;
}

/* Space Background */
.space-bg {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: radial-gradient(ellipse at bottom, #1B2735 0%, #090A0F 100%);
    z-index: -1;
}

/* Stars (Twinkling Effect) */
.stars {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><circle cx="10" cy="10" r="0.5" fill="white"/><circle cx="30" cy="20" r="0.7" fill="white"/><circle cx="70" cy="5" r="0.5" fill="white"/><circle cx="90" cy="30" r="0.8" fill="white"/><circle cx="50" cy="50" r="0.5" fill="white"/><circle cx="20" cy="70" r="0.7" fill="white"/><circle cx="80" cy="80" r="0.5" fill="white"/></svg>') repeat;
    animation: twinkle 4s infinite alternate;
}

@keyframes twinkle {
    0% { opacity: 0.5; }
    100% { opacity: 1; }
}

/* Sun (Center) */
.sun {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 80px;
    height: 80px;
    background: radial-gradient(circle, #FFD700, #FF8C00);
    border-radius: 50%;
    box-shadow: 0 0 50px #FF8C00;
    transform: translate(-50%, -50%);
    z-index: 1;
}

/* Planets */
.planet {
    position: absolute;
    border-radius: 50%;
    transform-origin: center;
}

.mercury {
    width: 10px;
    height: 10px;
    background: linear-gradient(to bottom, #A9A9A9, #696969);
    box-shadow: 0 0 10px #A9A9A9;
}

.venus {
    width: 15px;
    height: 15px;
    background: linear-gradient(to bottom, #E6E6FA, #9370DB);
    box-shadow: 0 0 10px #9370DB;
}

.earth {
    width: 18px;
    height: 18px;
    background: linear-gradient(to bottom, #1E90FF, #006400);
    box-shadow: 0 0 10px #1E90FF;
}

.mars {
    width: 14px;
    height: 14px;
    background: linear-gradient(to bottom, #FF6347, #8B0000);
    box-shadow: 0 0 10px #FF6347;
}

.jupiter {
    width: 30px;
    height: 30px;
    background: linear-gradient(to bottom, #F4A460, #CD853F);
    box-shadow: 0 0 15px #F4A460;
}

.saturn {
    width: 25px;
    height: 25px;
    background: linear-gradient(to bottom, #D2B48C, #A0522D);
    box-shadow: 0 0 15px #D2B48C;
}

/* Content Styling */
.content {
    position: relative;
    text-align: center;
    padding-top: 20vh;
    z-index: 10;
}

h1 {
    font-size: 3rem;
    text-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
}

p {
    font-size: 1.2rem;
    opacity: 0.8;
}
    
</head>
<body>

<div class="space-bg">
        <div class="stars"></div>
        <div class="sun"></div>
        <div class="planet mercury"></div>
        <div class="planet venus"></div>
        <div class="planet earth"></div>
        <div class="planet mars"></div>
        <div class="planet jupiter"></div>
        <div class="planet saturn"></div>
    </div>

    <h1 style="color: aliceblue">Hello everyone</h1>
    <h2 style="color: aliceblue">This is Rupayon</h2>
    <h3 style="color: aliceblue">Im 16 Years old </h3>
    <h3 style="font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif; color: aliceblue">Welcome to My website</h3>

    <p> I’m a student from the serene town of Kulaura, 
        and I’ve recently completed my Secondary School Certificate (SSC) examinations. 
        I aspire to become both an SEO specialist and a skilled programmer. Additionally, 
        I have a strong passion for artificial intelligence, which I find both 
        fascinating and full of potential.
</p>

        <p style="background-color: hwb(from color h w b); color: aliceblue;" >
While traditional books aren’t exactly my favourite, 
I thoroughly enjoy reading comics as a form of entertainment. 
In my leisure time, I love playing video games and going 
cycling with my friends. However, I’m not particularly 
fond of the scorching summer heat or gloomy rainy days.</p>
            <blockquote style="color: aliceblue">RUPAYON</blockquote>
            <p style="color: aliceblue"><abbr title="Rupayon Chakrabarty Sagor">RCS</abbr></p>
    <img ; src="IMG_9112.JPG" width="300">


    <h3 style="color: aliceblue">Here is my YouTube</h3>
    <a href="https://www.youtube.com/@Zero_Fame_YT"><h1 style="color: rgb(255, 255, 255);">Click here   (Youtube)</h1></a>
    <hr />
    <h3>Here is my Instagram</h3>
          <a href="https://www.instagram.com/rupayo_ngraphy?igsh=MWV3bTdrMWpkOXRlOA%3D%3D&utm_source=qr"><h1 style="color: rgb(255, 255, 255);">Click here</h1></a>
    <hr />
         <a href="about.html"><h1 style="color: rgb(255, 255, 255);">About Me</h1></a>
          <hr />

    <p>I learned </p>

    <ol>
          <li>CSS</li>
          <li>JS</li>
          <li>HTML</li>
          <li>Python</li>
      
    </ol>


                <head>
     

        document.addEventListener('DOMContentLoaded', () => {
    // Configuration for planets
    const planets = [
        { name: 'mercury', radiusRatio: 0.1, speed: 0.02, size: 10 },
        { name: 'venus', radiusRatio: 0.15, speed: 0.015, size: 15 },
        { name: 'earth', radiusRatio: 0.2, speed: 0.01, size: 18 },
        { name: 'mars', radiusRatio: 0.25, speed: 0.008, size: 14 },
        { name: 'jupiter', radiusRatio: 0.35, speed: 0.005, size: 30 },
        { name: 'saturn', radiusRatio: 0.45, speed: 0.003, size: 25 }
    ];

    // Store current angles and center position
    const angles = {};
    let mouseX = 0, mouseY = 0;
    let center = { x: 0, y: 0 };
    let minDimension = 0; // Used to scale orbits

    // Initialize angles and set planet sizes
    planets.forEach(planet => {
        angles[planet.name] = Math.random() * Math.PI * 2;
        const el = document.querySelector(`.${planet.name}`);
        el.style.width = `${planet.size}px`;
        el.style.height = `${planet.size}px`;
    });

    // Update center and orbit sizes on resize
    function updateDimensions() {
        center = {
            x: window.innerWidth / 2,
            y: window.innerHeight / 2
        };
        minDimension = Math.min(window.innerWidth, window.innerHeight);
        
        // Update sun position
        const sun = document.querySelector('.sun');
        sun.style.left = `${center.x}px`;
        sun.style.top = `${center.y}px`;
    }

    // Track mouse movement
    document.addEventListener('mousemove', (e) => {
        mouseX = e.clientX - center.x;
        mouseY = e.clientY - center.y;
    });

    // Handle window resize
    window.addEventListener('resize', updateDimensions);

    // Animation loop
    function animate() {
        const mouseDistance = Math.min(1, Math.sqrt(mouseX * mouseX + mouseY * mouseY) / (minDimension * 0.3));
        
        planets.forEach(planet => {
            const el = document.querySelector(`.${planet.name}`);
            
            // Update angle with speed and mouse influence
            angles[planet.name] += planet.speed * (1 + mouseDistance * 0.5);
            
            // Calculate orbit radius based on window size
            const radius = planet.radiusRatio * minDimension * 0.4;
            
            // Calculate circular position
            const x = center.x + Math.cos(angles[planet.name]) * radius;
            const y = center.y + Math.sin(angles[planet.name]) * radius;
            
            // Apply position
            el.style.left = `${x}px`;
            el.style.top = `${y}px`;
        });

        requestAnimationFrame(animate);
    }

    // Initialize and start animation
    updateDimensions();
    animate();
});
</body>


</html>
