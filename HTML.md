```html
<!DOCTYPE html>
<html lang="fr">
    <head>
        <!--déclarer l'encodage des caractères d'une page -->
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width,initial-scale=1.0">
        <!--Pour tout le réferencement-->
        <meta name="keywords" content="Devoir1"/>
        <meta name="robot" content="index"/>
        <meta name="description" content="Mais devoir 1"/>
        <!--Compatibilité IE et Edge-->    
        <meta http-equiv="X-UA-Compatible" content="ie=edge"/>
        <!--acces au document CSS-->
        <link rel="stylesheet" href="style/style.css" />
        <!--Ajouter une icon dans l'onglet-->
        <link rel="icon" href="ressources/mimi.jpg" type="image/jpg"/>
        <!--Titre de l'ongler-->
        <title>Titre de l'ongler</title>
    </head>
    <body>
        <!--Style de titre different/plus ou moins important niveaux sementique-->
        <h1>Titre</h1>
        <h2>Titre</h2>
        <h3>Titre</h3>
        <h4>Titre</h4>
        <h5>Titre</h5>
        <h6>Titre</h6>
        <!--Paragraphe (balise de style block)-->
        <p>Mon texte</p>
        <!--'ascii art' covertion du binaire en caractere ♥(alt+3)-->
         <pre>
            __ ___ ________ _||____|0| |Salut | &lt;_ __ _|- |_ __ _| 00 00 0 0 
        </pre>
        <!--signifie bloc de citation-->
         <blockquote cite="https://...">
        <p>
            Ceci est une citation 
        </p>
        </blockquote> 
        <!--Indique une portion de texte "décalée" du contenu principal (par défaut en italique) Ne dois plus etre utiliser-->
        <i>mon texte</i>
        <!--Indique une portion de texte affectée par une emphase. referencement (balise sementique) 'croll' robot de referencement-->
        <em>Mon texte</em>
        <!--gener un saut de ligne (balise orpheline)-->
        <hr>
        <!--utiliser quand il n'y a pas dautre balise de disponible.
        (principal de type de balise sementique)Balise four tout-->
        <div>Mon texte</div>
        <!--Utiliser surtout pour des liens-->
        <nav>Mon texte</nav>
        <!--Utiliser pour les partis independante-->
        <article>Mon texte</article>
        <!--Utiliser surtout pour les tables des matieres-->
        <section>Mon texte</section>
        <!--Utiliser pour les element secondaire les flux rss-->
        <aside>Mon texte</aside>
        <!--Utiliser pour les section principal utiliser pour le mode lecture (flux rss = alert pour les abonnée au flux rss, logiciel rss feed reader/mail)-->
        <main>Mon texte</main>
        <!--Lien dans un nouvelle ongler-->
        <a href="index2.html" target="_blank">Mon texte</a>
        <!--Liste ordonné-->
        <ol>
            <li>Rouge</li>
            <li>Noir</li>
            <li>bleu</li>
            <li>vert</li>
        </ol>
        <!--Liste désordoné-->
        <ul>
            <li>Rouge</li>
            <li>Noir</li>
            <li>Bleu</li>
            <li>Vert</li>
        </ul>
```
```html 
        <!--Les formulaires-->
        <!--action = vers ou l'envoier-->
        <form action="form.php" method="get">Mettre tout le formulaire à l'interieur</form>
        <!--placeholder est un attribut qui permet de renseigner un texte indicatif par défaut dans un champ de formulaire.
        C'est une valeur qui s'efface dès que l'utilisateur active le champ de formulaire (ou commence à écrire dedans si vous êtes sous Webkit).
        required = case obligatoire-->
        <input type="text/radio/checkbox/number" name="nom/radio" placeholder="mon texte" value="remplie automatiquement" required>
        <!--Pour avoir un grand texte-->
        <textarea name="texte">mon texte</textarea>
        <!--bouton envoyer-->
        <input type="submit"/>
        <!--Liste déroulante-->
        <select>
            <optgroup label="Nom de la liste">
                <option value="nom du bouton">nom du bouton</option>
                <option value="nom du bouton 2">nom du bouton 2</option>
                ....
        </select>
```
```html
        <!--Les tableaux-->
        <table>
            <!--représente la légende (ou le titre) d'un tableau-->
            <caption>Mon texte</caption>
            <!--en téte-->
            <thead>
                <!--ligne-->
                <tr>
                    <!--Ligne importante-->
                    <th>Mon texte</th>          
                </tr>
            </thead>
            <!--corp-->
            <tbody>
                <tr>
                    <!--colone-->
                    <td>Mon texte</td> 
                </tr>
            </tbody>
        </table>
```
```html
<!--Exemple tableau-->
    <h2>Tableau 6</h2>
    <table>
        <caption>Tableau 6</caption>
            <thead>
                <tr>
                    <th>1</th>
                    <th colspan="3">2</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td rowspan="3">3</td>
                    <td colspan="2">4</td>
                    <td rowspan="2">5</td>
                </tr>
                <tr>
                    <td rowspan="2">6</td>
                    <td>7</td>
                </tr>
                <tr>
                    <td colspan="2">8</td>
                </tr>
            </tbody>
    </table>
   _____________________ 
   |_1__|_______2______|
   |    |____4____| 5  |
   | 3  |6   |7___|____| 
   |____|____|____8____| 
    </body>
</html>
```