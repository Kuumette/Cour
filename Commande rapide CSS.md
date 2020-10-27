```CSS
________________
|              |
|______________|
|       |      |
|_______|______|

#entier {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-areas: 
    "haut haut"
    "gauche droite";  
}
#haut {
    grid-area: haut;
}
#gauche {
    grid-area: gauche;
}
#droite {
    grid-area: droite;
}
```
# HTML correspondant au CSS 
```HTML
<!DOCTYPE html>
<html lang="fr">
    <body>
        <div id="entier">
            <div id="haut">
                <h1>...</h1>
                <p>...</p>
            </div>

            <div id="gauche">
                <h2>...</h2>
                <p>...</p>
            </div>

            <div id="droite">
                <h2>...</h2>
                <p>...</p>
            </div>
        </div>
    </body>
</html>
```