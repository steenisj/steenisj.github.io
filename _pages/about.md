---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<h1>How many hotdogs should you eat today?</h1>

<!-- Button to trigger the estimator -->
<button id="hotdogButton">How Many?</button>

<!-- Element to display the output -->
<div id="output" style="margin-top: 20px; font-weight: bold;"></div>

<script>
    // Function to estimate hotdogs and play audio
    function hotdogEstimator() {
        console.log("hotdogEstimator function called!");

        // Generate a random number (1 to 10)
        var randomNumber = Math.floor(Math.random() * 10) + 1;

        // Play audio
        var audio = new Audio("{{ '/files/wiiSportsDiscChannel.mp3' | relative_url }}");

        audio.play().then(() => {
            console.log("Audio is playing.");
        }).catch((error) => {
            console.error("Error playing audio:", error);
        });

        // Display the output
        document.getElementById("output").innerHTML = 
            "You must eat " + randomNumber + " hotdogs today!";
    }

    // Attach event listener to the button
    document.getElementById("hotdogButton").addEventListener("click", hotdogEstimator);
</script>
