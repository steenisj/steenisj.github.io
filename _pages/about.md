---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<h1>How many hotdogs should you eat today?</h1>

<!-- Use a div or just a button without a form -->
<button onclick="hotdogEstimator()">How Many?</button>

<!-- Element to display the output -->
<div id="output" style="margin-top: 20px; font-weight: bold;"></div>

<script>
    function hotdogEstimator() {
        // Prevent any default form submission behavior if inside a form
        // Generate a random number
        var randomNumber = Math.floor(Math.random() * 10) + 1; // Random number between 1 and 10

        // Play audio
        var audio = new Audio("{{ '/files/wiiSportsDiscChannel.mp3' | relative_url }}");
        audio.play();

        // Display the output
        document.getElementById("output").innerHTML = 
            "You must eat " + randomNumber + " hotdogs today!";
    }
</script>
