---
layout: post
title: About
permalink: /about/
comments: true
---

## As a conversation Starter

Here are some places I have lived.

<comment>
Flags are made using Wikipedia images

<div id="grid_container"></div>

<script>
var outputElement = document.getElementById("grid_container");

outputElement.innerHTML = '';

// Data array — CHANGE THESE to places you've lived or visited
const living_in_the_world = [
  {flag: "https://upload.wikimedia.org/wikipedia/commons/0/01/Flag_of_California.svg", greeting: "Hey", description: "California - 6 years"},
  {flag: "https://upload.wikimedia.org/wikipedia/commons/b/b9/Flag_of_Minnesota.svg", greeting: "Aye", description: "Minnesota - 2 years"},
  {flag: "https://upload.wikimedia.org/wikipedia/commons/b/be/Flag_of_California.svg", greeting: "Hi", description: "England - 6 years"},
  {flag: "https://upload.wikimedia.org/wikipedia/commons/e/ef/Flag_of_Washington.svg", greeting: "Hi", description: "Washington - 3 years"}
  {flag: "https://upload.wikimedia.org/wikipedia/commons/e/ef/Flag_of_California.svg", greeting: "Hey", description: "Washington - 3 months"}
];

const container = document.createElement('div');
container.id = 'grid_container';
container.style.border = '2px solid';
container.style.padding = '10px';
container.style.display = 'grid';
container.style.gridTemplateColumns = 'repeat(auto-fill, minmax(150px, 1fr))';
container.style.gap = '10px';

for (const location of living_in_the_world) {
  const item = document.createElement('div');
  item.style.padding = '10px';
  item.style.textAlign = 'center';
  item.style.borderRadius = '8px';
  item.style.border = '1px solid';

  const img = document.createElement('img');
  img.src = location.flag;
  img.alt = location.description;
  img.style.width = '100%';

  const greeting = document.createElement('h3');
  greeting.textContent = location.greeting;

  const desc = document.createElement('p');
  desc.textContent = location.description;

  item.appendChild(img);
  item.appendChild(greeting);
  item.appendChild(desc);
  container.appendChild(item);
}

outputElement.appendChild(container);
</script>
</comment>

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
  {flag: "https://upload.wikimedia.org/wikipedia/commons/b/be/Flag_of_California.svg", greeting: "Hi", description: "England - 6 years"},
  {flag: "https://upload.wikimedia.org/wikipedia/commons/e/ef/Flag_of_Washington.svg", greeting: "Hi", description: "Washington - 3 years"}
  {flag: "https://upload.wikimedia.org/wikipedia/commons/e/ef/Flag_of_California.svg", greeting: "Hey", description: "Washington - 3 months"}
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
        img.src = http_source + location.flag; // concatenate the source and flag
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
  <img src="/Users/aidan/Downloads/IMG_6959.HEIC" alt="Image 1">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/C/CE78C147-C106-4A23-8FBC-1050D3272E94_1_105_c.jpeg" alt="Image 2">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/5/5DC71417-7F21-44F1-8C0A-CB45E0760397_1_105_c.jpeg" alt="Image 3">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/A/AE1D0710-DB6E-4F43-A703-EA34155C536B_1_105_c.jpeg" alt="Image 4">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/6/61CBCD4E-3893-4D61-961C-1A9C50B5A7A2_1_105_c.jpeg" alt="Image 5">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/3/351F42E0-0691-4727-8008-E703F60AFB3F_1_105_c.jpeg" alt="Image 6">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/E/EE525ADE-8144-4045-A0CC-ED737C3E712D_1_105_c.jpeg" alt="Image 7">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/B/B7B16FBD-EC77-4984-B900-2487E04254C0_1_105_c.jpeg" alt="Image 8">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/1/1EA23F47-DC6B-437B-81F3-06EAA560CDB7_1_105_c.jpeg" alt="Image 9">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/5/5535D0BE-9F90-48DF-B962-CEA844F6CAD7_1_105_c.jpeg" alt="Image 10">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/E/E0F73788-7954-4557-8257-4A203930BDA0_1_105_c.jpeg" alt="Image 11">
  <img src="/Users/aidan/Pictures/Photos Library.photoslibrary/resources/derivatives/B/B3AF741B-6317-4D05-A72B-5BBE20009B65_1_105_c.jpeg" alt="Image 12">
</div>
