---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

<p id="output">How many hotdogs should you eat today?</p>

<script>
    function hotdogEstimator() {
        // Prevent the form from submitting and refreshing the page
        //event.preventDefault();

        // Generate a random number
        //var randomNumber = Math.floor(Math.random() * 10) + 1; // Random number between 1 and 10

        // Play audio
        //var audio = new Audio("{{ '/files/wiiSportsDiscChannel.mp3' | relative_url }}");
        //audio.play();

        // Display the output
        document.getElementById("output").innerHTML = "You must eat ";// + randomNumber + " hotdogs today!";
    }
</script>

<button onclick="hotdogEstimator()">How Many?</button>

<!-- Element to display the output 
<div id="output" style="margin-top: 20px; font-weight: bold;"></div>-->
