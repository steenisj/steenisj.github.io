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
    document.addEventListener("DOMContentLoaded", function() {
        // Ensure the function is set up after the document is loaded
        document.querySelector("button").onclick = function() {
            document.getElementById("output").innerHTML = "You clicked the button!"; // Test message
        };
    });
</script>

<button>How Many?</button>
