# acerult24.github.io
Actresses' moments, all in one spot. Acerult24

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Slideshow</title>
    <style>
        #slideshow-container {
            max-width: 600px;
            position: relative;
            margin: auto;
        }

        .mySlides {
            display: none;
        }

        img {
            width: 100%;
        }
    </style>
</head>
<body>

<div id="slideshow-container">
    <div class="mySlides">
        <img src="image1.jpg" alt="Slide 1">
    </div>

    <div class="mySlides">
        <img src="image2.jpg" alt="Slide 2">
    </div>

    <!-- Add more slides as needed -->

    <div class="mySlides">
        <img src="image9.jpg" alt="Slide 9">
    </div>
</div>

<script>
    let slideIndex = 0;
    showSlides();

    function showSlides() {
        let i;
        const slides = document.getElementsByClassName("mySlides");

        for (i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";
        }

        slideIndex++;

        if (slideIndex > slides.length) {
            slideIndex = 1;
        }

        slides[slideIndex - 1].style.display = "block";

        // Change slide every 3 seconds (adjust as needed)
        setTimeout(showSlides, 3000);
    }
</script>

</body>
</html>
