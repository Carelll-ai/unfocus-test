<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unfocus Test</title>
</head>
<body>
    <h1>Unfocus Test</h1>
    <p id="status">Tab status: <strong>Focused</strong></p>
    <p id="counter">Unfocus count: 0</p>

    <script>
        let unfocusCount = 0;

        // Deteksi focus dan blur pada window (browser)
        window.addEventListener('focus', function() {
            document.getElementById('status').innerHTML = 'Tab status: <strong>Focused</strong>';
        });

        window.addEventListener('blur', function() {
            document.getElementById('status').innerHTML = 'Tab status: <strong>Unfocused</strong>';
            unfocusCount++;
            document.getElementById('counter').textContent = `Unfocus count: ${unfocusCount}`;
        });
    </script>
</body>
</html>statusElement.innerHTML = 'Tab status: <strong>Unfocused</strong>';
                unfocusCount++;
            } else {
                statusElement.innerHTML = 'Tab status: <strong>Focused</strong>';
            }

            counterElement.textContent = `Unfocus count: ${unfocusCount}`;
        });
    </script>
</body>
</html>
