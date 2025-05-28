---
title: "When Code Becomes Canvas: Creating Art with Algorithms"
description: "This post describes my experience creating with code."
publishDate: "28 Feb 2025"
tags: ["code", "art"]
updatedDate: 26 Feb 2025
---

There’s a unique thrill in making art that’s not drawn by hand but created through lines of code. It’s where logic meets imagination, and rules become brushes. For me, creative coding is the perfect way to explore both my technical and artistic sides — a place where I get to compose visuals as carefully as I compose software.

## The Spark: Inspiration Meets Code

My journey into algorithmic art started with photography. Capturing real-world moments felt incredible, but I wanted to push further — to create something new from scratch. Inspired by nature, geometry, and the dynamic patterns I see while traveling, I began experimenting with generative art using tools like p5.js and Three.js.

Each project starts as a simple idea or a feeling: maybe the randomness of a forest canopy or the rhythm of a city street. Then comes the challenge — how to translate that into code.

## The Creative Process

Unlike traditional art, where every stroke is deliberate, coding art involves embracing both structure and chance. I write algorithms that set the rules, but the results can surprise me every time. Sometimes a small tweak to a parameter creates a wave of unexpected beauty; other times, it reveals patterns I never planned.

Here’s a simple example: a grid of circles whose sizes and colors change based on a sine wave function. It’s mathematics creating movement and life on the screen.

```js
function setup() {
 createCanvas(400, 400);
 noLoop();
}

function draw() {
 background(255);
 let spacing = 40;
 for (let x = spacing / 2; x < width; x += spacing) {
  for (let y = spacing / 2; y < height; y += spacing) {
   let size = map(sin((x + y) * 0.1), -1, 1, 10, 30);
   fill(map(y, 0, height, 100, 255));
   ellipse(x, y, size);
  }
 }
}
```

## Why I Keep Coming Back

There’s a beautiful tension between control and unpredictability in creative coding. I get to design a system, but the final outcome often feels like a collaboration with the computer. It pushes me to think differently about problem-solving — seeing challenges as opportunities for exploration.

Plus, sharing these projects online — mixing visuals, code, and stories — lets me connect with a community of fellow creators who love pushing boundaries as much as I do.

## What’s Next?

I’m excited to dive deeper into 3D visualizations, interactive pieces, and maybe even combining photography with live code art. If you’re curious about any of this or want to try creative coding yourself, let me know! I’ll be sharing tutorials, tools, and my favorite resources here.
