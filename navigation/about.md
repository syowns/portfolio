---
layout: post
title: About
permalink: /about/
comments: true
---

## As a conversation Starter

Here are some places I have lived.


<style>
    /* Style looks pretty compact, 
       - grid-container and grid-item are referenced the code 
    */
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
</style>

<!-- This grid_container class is used by CSS styling and the id is used by JavaScript connection -->
<div class="grid-container" id="grid_container">
    <!-- content will be added here by JavaScript -->
</div>

<script>
    // 1. Make a connection to the HTML container defined in the HTML div
    var container = document.getElementById("grid_container"); // This container connects to the HTML div

    // 2. Define a JavaScript object for our http source and our data rows for the Living in the World grid
    var http_source = "https://upload.wikimedia.org/wikipedia/commons/";
    var living_in_the_world = [
          {flag: "https://upload.wikimedia.org/wikipedia/commons/0/01/Flag_of_California.svg", greeting: "Hey", description: "California - 6 years"},
  {flag: "https://upload.wikimedia.org/wikipedia/commons/b/b9/Flag_of_Minnesota.svg", greeting: "Aye", description: "Minnesota - 2 years"},
  {flag: "https://upload.wikimedia.org/wikipedia/commons/0/01/Flag_of_California.svg", greeting: "Hi", description: "California - 6 years"},
  {flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Flag_of_Washington.svg/3840px-Flag_of_Washington.svg.png?utm_source=en.wikipedia.org&utm_campaign=imageinfo&utm_content=thumbnail", greeting: "Hi", description: "Washington - 3 years"},
  {flag: "https://upload.wikimedia.org/wikipedia/commons/0/01/Flag_of_California.svg", greeting: "Hey", description: "California - 3 months"}
    ];

    // 3a. Consider how to update style count for size of container
    // The grid-template-columns has been defined as dynamic with auto-fill and minmax

    // 3b. Build grid items inside of our container for each row of data
    for (const location of living_in_the_world) {
        // Create a "div" with "class grid-item" for each row
        var gridItem = document.createElement("div");
        gridItem.className = "grid-item";  // This class name connects the gridItem to the CSS style elements
        // Add "img" HTML tag for the flag
        var img = document.createElement("img");
        img.src = location.flag; // concatenate the source and flag
        img.alt = location.flag + " Flag"; // add alt text for accessibility

        // Add "p" HTML tag for the description
        var description = document.createElement("p");
        description.textContent = location.description; // extract the description

        // Add "p" HTML tag for the greeting
        var greeting = document.createElement("p");
        greeting.textContent = location.greeting;  // extract the greeting

        // Append img and p HTML tags to the grid item DIV
        gridItem.appendChild(img);
        gridItem.appendChild(description);
        gridItem.appendChild(greeting);

        // Append the grid item DIV to the container DIV
        container.appendChild(gridItem);
    }
</script>

### Journey through Life

Here is what I did at those places

- ⛪ Shoal Creek Elementary School in San Diego(CA)
- ⛪ Excelsior Elementary School in Chanhassen(MN)
- ⛪ Turtleback Elementary School in San Diego(CA)
- ⛪ Bernardo Heights Middle School in San Diego(CA)
- 🔎 Competed in Science Olympiad
- ⛪ Evergreen Middle School in Redmond(WA)
- ⛪ Tesla STEM High School in Redmond(WA)
- 🤖 Competed in TSA, placed 7th in state for Robotics
- ⛪ Del Norte High School in San Diego(CA)

### Fun

Things I enjoy

- I play the guitar and enjoy listening to rock, mountain bike, hike- hopefully I'll be able to hike El Cajon this year, and buy & sell sports cards

<comment>
Gallery of Pics, scroll to the right for more ...
</comment>
<div class="image-gallery">
  <img src="{{site.baseurl}}/images/about/photo1.jpg" alt="Image 1">
  <img src="{{site.baseurl}}/images/about/photo2.jpg" alt="Image 2">
  <img src="{{site.baseurl}}/images/about/photo3.jpg" alt="Image 3">
  <img src="{{site.baseurl}}/images/about/photo4.jpg" alt="Image 4">
  <img src="{{site.baseurl}}/images/about/photo5.jpg" alt="Image 5">
  <img src="{{site.baseurl}}/images/about/photo6.jpg" alt="Image 6">
  <img src="{{site.baseurl}}/images/about/photo7.jpg" alt="Image 7">
  <img src="{{site.baseurl}}/images/about/photo8.jpg" alt="Image 8">
  <img src="{{site.baseurl}}/images/about/photo9.jpg" alt="Image 9">
  <img src="{{site.baseurl}}/images/about/photo10.jpg" alt="Image 10">
  <img src="{{site.baseurl}}/images/about/photo11.jpg" alt="Image 11">
  <img src="{{site.baseurl}}/images/about/photo12.jpg" alt="Image 12">
</div>
