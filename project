<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Galerie de Photos Interactive</title>
    <style>
        #image {
            width: 500px;
            height: 300px;
            background-color: lightgray;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            font-size: 18px;
            font-family: Arial, sans-serif;
            margin-bottom: 20px;
        }
        .preview {
            margin: 10px;
            width: 100px;
            height: 100px;
            cursor: pointer;
        }
        figure {
            display: inline-block;
            margin: 10px;
        }
        figcaption {
            text-align: center;
        }
    </style>
</head>
<body onload="initializeTabFocus()">
    <h1>Galerie de Photos Interactive</h1>
    <div id="image">Hover over an image below to display here</div>

    <section id="gallery">
        <figure>
            <img class="preview" src="image1.jpeg" alt="Description of Image 1" onmouseover="upDate(this)" onmouseout="unDo()" onfocus="upDate(this)" onblur="unDo()">
            <figcaption>Image 1</figcaption>
        </figure>
        <figure>
            <img class="preview" src="image2.jpeg" alt="Description of Image 2" onmouseover="upDate(this)" onmouseout="unDo()" onfocus="upDate(this)" onblur="unDo()">
            <figcaption>Image 2</figcaption>
        </figure>
        <figure>
            <img class="preview" src="image3.jpeg" alt="Description of Image 3" onmouseover="upDate(this)" onmouseout="unDo()" onfocus="upDate(this)" onblur="unDo()">
            <figcaption>Image 3</figcaption>
        </figure>
   
    </section>

    <script>
        // Fonction appelée au survol ou focus d'une image
        function upDate(previewPic) {
            const displayDiv = document.getElementById("image");
            displayDiv.style.backgroundImage = url(${previewPic.src});
            displayDiv.textContent = previewPic.alt;
        }

        // Fonction appelée à la sortie ou perte de focus
        function unDo() {
            const displayDiv = document.getElementById("image");
            displayDiv.style.backgroundImage = "none";
            displayDiv.textContent = "Hover over an image below to display here";
        }

        // Fonction exécutée au chargement de la page pour ajouter tabindex
        function initializeTabFocus() {
            console.log("Adding tabindex attributes");
            const images = document.querySelectorAll('.preview');
            for (let i = 0; i < images.length; i++) {
                images[i].setAttribute('tabindex', '0');
            }
        }
    </script>
</body>
</html>
