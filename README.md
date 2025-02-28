<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Głośna Strona</title>
</head>
<body>
    <h1>Witamy na bardzo głośnej stronie!</h1>
    <audio id="audio" src="audio.mp3" preload="auto" loop>
        Twoja przeglądarka nie wspiera tagu audio.
    </audio>
    <script>
        // Pobranie elementu audio
        var audio = document.getElementById("audio");
        
        // Ustawienie maksymalnej głośności
        audio.volume = 1;  // 1 to maksymalna głośność (0 - 1)

        // Rozpoczęcie odtwarzania dźwięku od razu po załadowaniu strony
        audio.play();
    </script>
</body>
</html>
