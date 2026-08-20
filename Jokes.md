```python
---
layout: post
toc: True
breadcrumb: True
title: GitHub Pages Jokes 
description: These Programming topics are focused on Jupyter Notebooks, and Managing Files.
permalink: /github/pages/jokes
author: John Mortensen
---

```

## Running Jupyter Notebooks

Let's have a laugh while we test out JavaScript in Jupyter Notebooks.

- In VSCode, go to **Help->Toggle Developer Tools**
- Click on **Console** in the newly opened Window
- Clear screen by pressing **Clear Console** (circle with line)
- Then press **Play button** to left of cells below
- Observe random output in the Console


### Programmer Jokes

An array of key-value pairs (JavaScript objects). Each joke has a "complexity" rating—if you understand the ones rated "3," your teacher will be impressed!

```javascript
%%javascript

var compsci_joke_list = [
    { joke: "Why do programmers prefer dark mode? Because light attracts bugs.", complexity: "1" },
    { joke: "Why do Java developers wear glasses? Because they don't see sharp.", complexity: "2" },
    { joke: "How many programmers does it take to change a light bulb? None, that's a hardware problem.", complexity: "1" },
    { joke: "Why do Python programmers prefer snake_case? Because they can't C.", complexity: "2" },
    { joke: "Why was the JavaScript developer sad? Because he didn't know how to 'null' his feelings.", complexity: "3" },
    { joke: "Why do programmers always mix up Christmas and Halloween? Because Oct 31 == Dec 25.", complexity: "3" },
    { joke: "Why did the programmer quit his job? Because he didn't get arrays.", complexity: "O(n)" },
    { joke: "Why do Linux programmers prefer using the terminal? Because they don't like Windows.", complexity: "1" },
];
var randomIndex = Math.floor(Math.random() * compsci_joke_list.length);
var selectedJoke = compsci_joke_list[randomIndex];
console.log("Joke #" + (randomIndex + 1) + ": " + selectedJoke.joke + " (Complexity: " + selectedJoke.complexity + ")");
```

### Accountant Jokes

A simpler array of strings—these jokes are just plain text, not JavaScript objects.

```javascript
%%javascript

var accounting_joke_list = [
    "Why did the accountant cross the road? To bore the people on the other side.",
    "What do accountants do when they're constipated? They work it out with a pencil.",
    "How does an accountant stay out of debt? He learns to act his wage.",
    "Why did the accountant stare at his glass of orange juice for three hours? Because on the box it said 'concentrate'.",
    "Why did the accountant get promoted? Because he knew how to balance his work and play.",
    "Why did the accountant go broke? Because he lost his balance.",
    "Why did the accountant get a job at the bakery? Because he was good at making dough.",
    "Why did the accountant get a job at the zoo? Because he was good with cheetahs.",
    "Why did the accountant get a job at the library? Because he was good at keeping books.",
    "Why did the accountant get a job at the circus? Because he was good at juggling numbers.",
    "Why did the accountant get a job at the gym? Because he was good at working out the numbers.",
    "Why did the accountant get a job at the farm? Because he was good at counting the chickens before they hatched."
]
var randomIndex = Math.floor(Math.random() * accounting_joke_list.length);
console.log("Joke #" + (randomIndex + 1) + ": " + accounting_joke_list[randomIndex]);
```

### Fun Jokes Implementation With HTML

```html
%%html
<div style="text-align:center; padding:20px;">
    <h3>🎓 CS Joke Machine 🎓</h3>
    <div id="joke_box" style="font-size:18px; font-family:monospace; margin:20px; padding:15px; border-radius:12px; background:#222; color:#ffd700; min-height:60px; transition:background 0.5s;">
        Click the button for a joke!
    </div>
    <button onclick="showJoke()" style="padding:10px 20px; font-size:16px; border:none; border-radius:8px; background:#4CAF50; color:white; cursor:pointer;">Tell me a Joke 😄</button>
</div>

<script>
var cs_jokes = [
    { joke: "Why was the computer cold? Because it left its Windows open.", topic: "Operating Systems" },
    { joke: "Why did the student eat his homework? Because the teacher said it was a piece of cake.", topic: "School" },
    { joke: "Why do computers love snacks? Because they love microchips.", topic: "Hardware" },
    { joke: "What’s a computer’s favorite type of music? Algorithms and blues.", topic: "Algorithms" },
    { joke: "Why was the math book sad? Because it had too many problems.", topic: "Math" },
    { joke: "Why don’t robots ever get lost? Because they follow their GPS perfectly.", topic: "AI" },
    { joke: "What did the computer say to the keyboard? You’re my type!", topic: "Hardware" },
    { joke: "Why do programmers always carry a pencil? In case they need to draw a byte.", topic: "Programming" }
];

function typeWriter(text, elementId, i=0) {
    if (i < text.length) {
        document.getElementById(elementId).innerHTML += text.charAt(i);
        setTimeout(() => typeWriter(text, elementId, i + 1), 40);
    }
}

function showJoke() {
    var randomIndex = Math.floor(Math.random() * cs_jokes.length);
    var jokeObj = cs_jokes[randomIndex];

    // change box color randomly
    var colors = ["#222","#333","#2a2a2a","#111"];
    document.getElementById("joke_box").style.background = colors[Math.floor(Math.random() * colors.length)];

    // clear and add typing effect
    var box = document.getElementById("joke_box");
    box.innerHTML = "";
    var text = "💡 [" + jokeObj.topic + "] " + jokeObj.joke;
    typeWriter(text, "joke_box");
}
</script>
```

## Check out Tools for Jupyter Notebooks

Here are some diagnostics if notebooks above are not working.

```bash
%%script bash

# 🎨 Colors
RED='\033[0;31m'
GREEN='\033[0;32m'
YELLOW='\033[1;33m'
BLUE='\033[1;34m'
CYAN='\033[1;36m'
RESET='\033[0m'

# Array of commands
commands=("python --version" "jupyter --version" "jupyter kernelspec list")

# Pretty header
echo -e "${CYAN}"
echo "=============================================="
echo " 🚀  Environment Version Check Dashboard  🚀 "
echo "=============================================="
echo -e "${RESET}"

# Loop through commands
for cmd in "${commands[@]}"; do
  echo -e "${YELLOW}▶ Command:${RESET} ${BLUE}$cmd${RESET}"
  echo -e "${GREEN}Output:${RESET}"
  echo "----------------------------------------------"
  bash -c "$cmd"
  echo -e "${CYAN}----------------------------------------------${RESET}"
  echo
done

# Done message
echo -e "${GREEN}✅ Version check complete!${RESET}"
```

## Hack 

If you love these jokes, you’ll probably want to have them in your own repository. Learning how to manage files in GitHub Pages is a key skill. This class will continually share files and offer challenges using GitHub Pages and Jupyter Notebooks.


- How to copy files between two GitHub repositories
  - **git clone** pages repository to your machine
  - **git pull** if you already have it, un git pull to make sure your repository is up to date
  - **code .** in directory of the project directory where you cloned the repo 
  - **drag and drop** files between repositories, be sure to put them in the right type of folder 

### Tip

- The **_notebooks** directory is the default location to place all **.ipynb** files.  
  - To get started, you can copy **_notebooks/Foundation/C-github_pages** to your project.
  - Then, rename or modify these files as part of the hack.

- The **_notebooks/Foundations/C-github_pages** contains the files that use an InfoGraph for a menu
  - In **frontmatter** of each file you will find data that describes its prooperties. 
    - **permalink: /github/pages/intro** 
    - [Describe some other properties]

- Create a new cell with your own (PG-13 rated) jokes
  - Pick your own topic
  - Jokes could be a great warmup at next live review
