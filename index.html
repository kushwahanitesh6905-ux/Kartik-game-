<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Car Game</title>
    <style>
        body {
            margin: 0;
            background-color: #222;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            color: white;
            font-family: Arial, sans-serif;
            overflow: hidden;
        }
        canvas {
            border: 4px solid white;
            background-color: #333;
        }
    </style>
</head>
<body>

    <canvas id="gameCanvas" width="400" height="600"></canvas>

    <script>
        const canvas = document.getElementById("gameCanvas");
        const ctx = canvas.getContext("2d");

        // Car ki details
        let car = {
            x: 175,
            y: 500,
            width: 50,
            height: 80,
            speed: 5,
            color: "red"
        };

        // Obstacle (Dusri gaadi) ki details
        let obstacle = {
            x: Math.random() * 350,
            y: -100,
            width: 50,
            height: 80,
            speed: 4,
            color: "yellow"
        };

        let score = 0;
        let isGameOver = false;

        // Keyboard controls
        let keys = {};

        window.addEventListener("keydown", (e) => {
            keys[e.key] = true;
        });

        window.addEventListener("keyup", (e) => {
            keys[e.key] = false;
        });

        // Game loop
        function update() {
            if (isGameOver) return;

            // Car movement (Left/Right arrow keys)
            if (keys["ArrowLeft"] && car.x > 0) {
                car.x -= car.speed;
            }
            if (keys["ArrowRight"] && car.x < canvas.width - car.width) {
                car.x += car.speed;
            }

            // Obstacle movement
            obstacle.y += obstacle.speed;
            if (obstacle.y > canvas.height) {
                obstacle.y = -100;
                obstacle.x = Math.random() * (canvas.width - obstacle.width);
                score += 10;
                obstacle.speed += 0.2; // Jaise jaise score badhega, speed badhegi
            }

            // Collision detection (Takkar check karna)
            if (
                car.x < obstacle.x + obstacle.width &&
                car.x + car.width > obstacle.x &&
                car.x < obstacle.x + obstacle.width && // extra safety check
                car.y < obstacle.y + obstacle.height &&
                car.y + car.height > obstacle.y
            ) {
                isGameOver = true;
            }
        }

        function draw() {
            // Screen clear karein
            ctx.clearRect(0, 0, canvas.width, canvas.height);

            // Road ki lines draw karein
            ctx.strokeStyle = "white";
            ctx.setLineDash([20, 20]);
            ctx.beginPath();
            ctx.moveTo(200, 0);
            ctx.lineTo(200, canvas.height);
            ctx.stroke();

            // Player ki Car draw karein
            ctx.fillStyle = car.color;
            ctx.fillRect(car.x, car.y, car.width, car.height);

            // Obstacle Car draw karein
            ctx.fillStyle = obstacle.color;
            ctx.fillRect(obstacle.x, obstacle.y, obstacle.width, obstacle.height);

            // Score display karein
            ctx.fillStyle = "white";
            ctx.font = "20px Arial";
            ctx.fillText("Score: " + score, 20, 30);

            // Game Over message
            if (isGameOver) {
                ctx.fillStyle = "rgba(0, 0, 0, 0.7)";
                ctx.fillRect(0, 0, canvas.width, canvas.height);

                ctx.fillStyle = "red";
                ctx.font = "30px Arial";
                ctx.fillText("Game Over!", 120, 250);

                ctx.fillStyle = "white";
                ctx.font = "18px Arial";
                ctx.fillText("Refresh to Play Again", 110, 300);
            }
        }

        function loop() {
            update();
            draw();
            if (!isGameOver) {
                requestAnimationFrame(loop);
            }
        }

        loop();
    </script>
</body>
</html>
