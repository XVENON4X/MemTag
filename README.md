<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Głośna Strona</title>
</head>
<body>
    <h1>Witamy na bardzo głośnej stronie!</h1>
    <audio id="audio" src="audio.mp3" preload="auto" loop muted>
        Twoja przeglądarka nie wspiera tagu audio.
    </audio>

    <script>
        // Pobranie elementu audio
        var audio = document.getElementById("audio");

        // Rozpoczęcie odtwarzania dźwięku z wyciszeniem
        audio.play();

        // Ustawienie maksymalnej głośności
        audio.volume = 1;  // 1 to maksymalna głośność (0 - 1)

        // Po 1 sekundzie odmutowanie dźwięku
        setTimeout(function() {
            audio.muted = false;
        }, 1000);  // 1000 ms = 1 sekunda
    </script>
</body>
</html>
