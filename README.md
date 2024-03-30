# Slot-machine-
Slot Machine
<!DOCTYPE html>
<html>
<head>
    <title>Slot Machine</title>
</head>
<body>
    <h1>Slot Machine</h1>
    <p>Press the button to spin the slot machine!</p>
    
    <button onclick="spin()">Spin</button>
    
    <p id="result"></p>
    
    <script>
        function spin() {
            var symbols = ["Cherry", "Orange", "Lemon", "Apple", "Banana"];
            var result = [];
            
            for (var i = 0; i < 3; i++) {
                var randomIndex = Math.floor(Math.random() * symbols.length);
                result.push(symbols[randomIndex]);
            }
            
            document.getElementById("result").innerHTML = "Result: " + result.join(" - ");
        }
    </script>
</body>
</html>
