---
layout: page
title: SDLC
description: Showcase of how SDLC works
permalink: /sdlc/
---

I use SDLC for projects that I build for my portfolio. And these are the processes I go through when I'm building something.
<pre>
+-------------------+       +-------------------+       +-------------------+       +-------------------+       +-------------------+
|                   |       |                   |       |                   |       |                   |       |                   |
|   Make Server     | ----> |   Change Code     | ----> |     Commit        | ----> |      Test         | ----> |     Sync          |
|                   |       |                   |       |                   |       |                   |       |                   |
+-------------------+       +-------------------+       +-------------------+       +-------------------+       +-------------------+
        |                           |                           |                           |                           |
        v                           v                           v                           v                           v
 Start Local Server           Edit Code Files           Stage Changes Locally        Verify Local Changes        Push Changes to Cloud
 </pre>

### Planning

---

>What's the problem? Who's it for? What are the requirements? How long will it take? How much will it cost?

### Design

---

>How will it work? What data is being stored? What talks to what? What's being outputted?

### Development

---

>Process of writing the code, following the design.

### Testing

---

>Run the software and try to break it. Does it pass all requirements made in the planning stage? Does the program crash with weird inputs? Bug finding stage. Often steps **3→4→3→4→3→4**. Use of `make` to test on clientside.

### Deployment

---

>Pushing it to the live build so others can use it. `git push` sends the new build to Github pages, making the live build visible.

### Cycle

---

>Its a cycle because as new problems or goals are made, the whole cycle is repeated

