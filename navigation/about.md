---
layout: post
title: About Me 
description: My name is Arshia Deb Roy.
permalink: /about/
comments: true
---

<style>
    
    .grid-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic columns */
        gap: 10px;
    }
    .grid-item {
        text-align: center;
    }
    .grid-item img {
        width: 100%;
        height: 100px; /* Fixed height for uniformity */
        object-fit: contain; /* Ensure the image fits within the fixed height */
    }
    .grid-item p {
        margin: 5px 0; /* Add some margin for spacing */
    }

    .image-gallery {
        display: flex;
        flex-wrap: nowrap;
        overflow-x: auto;
        gap: 10px;
        }

    .image-gallery img {
        max-height: 150px;
        object-fit: cover;
        border-radius: 5px;
    }
    .image-flag img {
        max-height: 100px;
        max-width: 100px;
        border-radius: 5px;
    }
    .imageflag {
        width: 200px;
        height: 200px;
    } 
    .image-row {
        text-align: left;
        display: flex;
        gap: 1px;
        justify-content: space-between; /* this will add equal space between each image */
    }    

</style>

## Culture and Family

<!-- This grid_container class is used by CSS styling and the id is used by JavaScript connection -->
<div class="arshia-grid-container" id="arshia-grid-container">
    <!-- content will be added here by JavaScript -->
</div>

<script>

    console.log("I am working 1");
    var container = document.getElementById("arshia-grid-container");
    // var container = document.createElement("div");
    
    var http_source = "https://upload.wikimedia.org/wikipedia/commons/";
    var living_in_the_world = [
		{"flag": "4/41/Flag_of_India.svg", "greeting": "Namaste", "description": "India - Land Of Diversity"},
        {"flag": "0/01/Flag_of_California.svg", "greeting": "Hi", "description": "California - The golden State"},
    ];
        
    console.log("I am working 2");
    for (const location of living_in_the_world) {
        console.log("I am working 3");
        // Create a "div" with "class grid-item" for each row
        var gridItem = document.createElement("div");
        gridItem.className = "grid-item";  // This class name connects the gridItem to the CSS style elements
        // Add "img" HTML tag for the flag

        console.log("I am working 4");
        var img = document.createElement("img");
        img.src = http_source + location.flag; // concatenate the source and flag
        img.alt = location.description + " Flag"; // add alt text for accessibility

        console.log("I am working 5");
        // Add "p" HTML tag for the description
        var description = document.createElement("p");
        description.textContent = location.description; // extract the description

        console.log("I am working 6");
        // Add "p" HTML tag for the greeting
        var greeting = document.createElement("p");
        greeting.textContent = location.greeting;  // extract the greeting
        console.log("I am working 7");
        // Append img and p HTML tags to the grid item DIV
        gridItem.appendChild(img);
        gridItem.appendChild(description);
        gridItem.appendChild(greeting);

        // Append the grid item DIV to the container DIV
        console.log("I am working 8");
        container.appendChild(gridItem);
        console.log("I am working 9");
    }
</script>

Even though I am born in California, my family comes from India. I am very connected to my cuture and I regularly visit India and I do indian classical singing.
    

# Art 

I am also really into art and I took AP studio art last year at Del Norte. Here is some of my art. 

<comment>
Gallery of Pics, scroll to the right for more ...
</comment>
<div class="image-gallery">
  <img src="{{site.baseurl}}/images/about/arshiaart1.jpg" alt="Image 1">
  <img src="{{site.baseurl}}/images/about/arshiaart2.jpg" alt="Image 2">
  <img src="{{site.baseurl}}/images/about/arshiaart3.jpg" alt="Image 3">
  <img src="{{site.baseurl}}/images/about/arshiaart4.jpg" alt="Image 4">
  <img src="{{site.baseurl}}/images/about/arshiaart5.jpg" alt="Image 5">
</div>

# Fun Facts 

🐈 I really love cats and I want a cat in the future. 

🌊 I love to go to the beach. 

✨ I am trilingual and can speak english, hindi, and bengali. 

🥑 I love avocados and put them on everything. 

<script src="https://utteranc.es/client.js"
        repo="nighthawkcoders/portfolio_2025"
        issue-term="title"
        label="blogpost-comment"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script>
-->
