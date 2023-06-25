# GTKind.github.io
`AI for people of goodwill`
`Goodwill encompasses attitudes and actions that reflect love, kindness, righteousness, integrity, and the pursuit of peace. It emphasizes the importance of treating others with respect, compassion, and fairness, aligning with the teachings and values found in the Scriptures.`
<!DOCTYPE html>
<html>
<head>
    <title>Current Time</title>
    <style>
        body {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 10em;
            font-family: Arial, sans-serif;
        }
    </style>
    <script>
        function updateTime() {
            var date = new Date();
            var hours = date.getHours().toString().padStart(2, '0');
            var minutes = date.getMinutes().toString().padStart(2, '0');
            var seconds = date.getSeconds().toString().padStart(2, '0');
            var time = hours + ':' + minutes + ':' + seconds;
            document.body.textContent = time;
        }
        
        setInterval(updateTime, 1000); // Update time every second
    </script>
</head>
<body>
</body>
</html>

<html>
<head>
    <title>Color Changing Screen</title>
    <style>
        body {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: #000;
            transition: background-color 1s;
        }
    </style>
    <script>
        function changeColor() {
            var colors = ['#ff0000', '#00ff00', '#0000ff', '#ffff00', '#ff00ff', '#00ffff'];
            var body = document.querySelector('body');
            var currentColor = body.style.backgroundColor;
            var index = colors.indexOf(currentColor);
            var nextIndex = (index + 1) % colors.length;
            body.style.backgroundColor = colors[nextIndex];
        }
        
        setInterval(changeColor, 2000); // Change color every 2 seconds
    </script>
</head>
<body>
</body>
</html>
