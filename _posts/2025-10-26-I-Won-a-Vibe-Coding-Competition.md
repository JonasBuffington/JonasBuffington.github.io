---
layout: post
title:  "I Won a Vibe-Coding Competition. Here's Why I Had to Stop."
date:   2025-10-25 11:00:00 -0500
---
---

## Part 1: The Victory and the Paradox

The email landed in the inbox of every student in my university's computer science department. A 24-hour AI coding competition was announced. The challenge was to solve a complex combinatorial search problem. But the real test was the core constraint: the entire submission had to be the output of a single, final prompt to ChatGPT.



On the surface, it sounds like a pure test of prompt engineering. A search for that one magic incantation. It's the kind of task that encourages a vibecoding approach, rapidly iterating on phrasing, tweaking parameters, and chasing a lucky breakthrough until the AI spits out something that works.



But I had just spent two weeks learning that when it comes to building something robust, luck has nothing to do with it.



So I took a different path. For eighteen hours, I didn't search for a magic prompt. I engaged in a methodical, structured dialogue with the AI. I made it plan, challenged its assumptions, and forced it to reason through the entire prompt with me. The final prompt wasn't a stroke of luck or genius. It was the distilled summary of that entire conversation.



The code it produced was very efficient. It tore through a 20^10 search space in 1.3 seconds, identifying the optimal solution in just one millisecond and spending the rest of the time proving its own correctness.



A day later, I learned I had won. But the victory felt like less of a triumph of prompt-crafting and more like a validation of a lesson. That single, winning prompt was just the tip of the iceberg, resting on a massive, unseen foundation of disciplined work. A foundation I had been forced to build on a completely different project, one that taught me the real cost of relying on the vibe in vibecoding.



## Part 2: Forging the Method

A few weeks earlier, I wasn't thinking about competitions. I was deep in the trenches of a personal passion project: building a fully dynamic voxel destruction engine on Roblox. The dream was ambitious, to create a system where every object could be fractured in real-time, with the new geometry perfectly meshed. As a junior developer, I knew this was a big task, so I turned to an AI partner to get started.



In the beginning, it felt like a superpower. The AI churned out prototypes, implemented complex logic, and got me to a semi-functional state faster than I could have imagined. It was dangerously easy to fall into that pure vibecoding workflow.



That initial speed came at a hidden cost: architectural rot. I quickly learned that AI is a brilliant sprinter but blind when an architect. It can generate a script that *feels* right in isolation, but it struggles to build a coherent, scalable system. The tech debt piled up silently.



At first, this felt like an issue on my part. I thought I could prompt my way out of it. I became meticulous, demanding the AI to plan its changes, and I inspected every line of its output. For a while, it worked. The tech debt seemed to melt away, and I felt I had mastered the hardest part of the workflow.



I was wrong. I hadn't solved the entire problem. I had only reached a higher, harder wall. Something I found as a great filter of AI-assisted development: platform specific reality.



It starts with a bug the AI can't fix or a feature it can't implement. You describe the problem perfectly, but the AI's solutions don't cut it, no matter how sensible they sound. It seems to brute-force solutions, or take the longest path to a solution imaginable. This is the moment you realize the AI's vast knowledge is a mile wide and an inch deep. It cannot understand the nuances that make or break a project, and no amount of clever prompting can bridge that gap.



This filter however wasn't one single thing, but a combination of hard limitations I was forced to confront and solve myself:



* **The Token Window**: The AI's memory is finite. As the project grew, I had less and less room to provide the necessary context before it's performance began to degrade. It's like trying to explain a whole book to someone who can only remember the past 30 seconds.

* **The API Gap**: The AI knew of some of Roblox's APIs, but it didn't *fully understand* them. It couldn't discern the efficient and modern solutions from a slow legacy method. It would consistently choose brute-force solutions over elegant, engine-native ones.

* **The Physics of the Platform**: The most stubborn bugs were rooted in the unique behavior of Roblox's physics engine, and the overhead of it's methods. This was knowledge that simply didn't exist enough in the AI's training data. It was a context I couldn't provide because I first had to learn it myself.



The vibe was gone, the superpower had failed. To move forward, I had to stop being a prompter and start being an engineer. I had to gain some expertise.



Hitting that wall wasn't a failure but a diagnosis. It revealed the fundamental flaw in my approach. I had been treating AI as an oracle, a black box that held the answers. The epiphany was realizing that I needed to treat it like a brilliant but amnesiac intern. It has immense raw capability but no context, no wisdom, and no real understanding of the specific world it's working in. My job wasn't to ask it for answers, but to provide it with the framework to build them.



This changed everything. I developed a new, disciplined workflow built on three core principles, each one a direct response to the filter that had stopped me cold:



* **To solve the Token Window, I became a curator.** Instead of dumping the entire project on the AI's desk, I learned to perform surgical insertions. I abstracted my code into smaller, more digestible modules and created a simplified API "cheat sheet" for the AI to reference. I was actively managing the AI's "cognitive load"



* **To bridge the API Gap, I became the expert.** I spent hours scouring forums and documentation, not looking for code to copy, but for principles to understand. "Fix this bug" became "Refactor this module to use the BulkMoveTo method, because it's more performant for batch operations than moving parts individually," I was no longer asking for its knowledge, I began injecting my own.

* **And to solve the impossible bugs, I became a Socratic partner.** I stopped asking for solutions and started demanding explanations. "Explain your reasoning." "Why did you choose that data structure?" "Walk me through the logic of this function line by line." More often than not, in forcing the AI to articulate its flawed logic, I would spot the error myself. The dialogue wasn't about getting a fix, it was about building a shared understanding.



The AI was no longer a magic wand I was waving at a problem. It was a tool and force multiplier for my own personal engineering process. The goal shifted from getting a working output to building a robust, comprehensible system. And that discipline, created in the frustrating voxel engine problem, was the exact weapon I needed for the competition that was just around the corner.



## Part 3: The Proving Ground

When the competition began, my first three hours were spent away from the keyboard. While others were likely already deep into the rapid cycle of prompting and testing, I was exercising the first lesson from the voxel engine: you cannot prompt your way out of a problem you don't fully understand. I spent that time decomposing the problem, identifying the constraints, and mapping out the steps needed to arrive at an optimal solution. I wasn't just planning my prompt, I was creating a  technical blueprint for the AI to follow.

Only after this did I open the chat window. The next fifteen hours were the methodical execution of the workflow I had forged.

First, I acted as the expert. I didn't ask the AI how to solve the problem. I told it. I fed my decomposed plan, outlined the most efficient algorithms for this type of search, and provided the specific mathematical constraints it had to respect. I was front loading the inch deep knowledge it lacked.

Then, I began a modified version of the Socratic dialogue. I'd command it to generate a plan and implement the logic. I'd make a branch of the chat and ask it why it chose certain implementations, learning from it's choices to inform my own for subsequent attempts. I went back and forth like this, essentially arguing over implementation details and edge cases. I was stress testing the logic of alternate timelines, due to the constraint that the problem must be finished in one prompt. This was a deliberately slow grind towards an optimal solution and an optimal prompt, the polar opposite of vibecoding.



Finally, I became the curator. When I knew my plan was solid, the task shifted to condensing all that I had learned about the problem into a single, perfect set of instructions. This took meticulous iteration over my existing prompt to strive for a more efficient communication for the LLM to digest.



When I finally hit enter on that last prompt, it didn't feel like a gamble. It felt like an inevitability. The code that appeared on the screen wasn't a lucky guess from a black box, it was the logical output of a disciplined and rigorous engineering process, a process where I was the architect and the client.



## Part 4: The Real Prize

The real prize of the competition wasn't the win. It was the validation. It was the definitive proof that the painfully slow and deliberate method I had forged in the development of the voxel engine wasn't just a coping mechanism but a superior strategy.



The tech world is obsessed with the idea that AI coding will make everyone into a "10x engineer" or that it will "1.5x your efficiency." My experience suggests that this is a dangerous misconception, the idea that AI will simply and easily improve your speed is a siren's call that leads to shallow understanding and fragile results. I believe chasing true 10x efficiency with AI is a fool's errand. It encourages you to become a passenger, to vibe check a black box and hope for the best.



The true power of this technology, especially for a learner, isn't 10x efficiency. It's 10x learning.



The AI's real value isn't in giving you answers. It's in creating a feedback loop for your own mind. It forces you to articulate your assumptions with perfect clarity. It exposes your knowledge gaps with precision when it produces nonsense. It provides a consequence free sandbox to debate complex architectural decisions. This is where the line is drawn between a tool and a crutch. A tool multiplies your existing capability, allowing you to build better and faster. A crutch allows you to bypass developing that capability in the first place. Pure vibecoding is leaning on the crutch.



After this journey, I still believe that using AI to code has no hard technical limitations. But now I see the true limitation is not in the machine, but in the user. It is the limitation of our own discipline. The AI will happily let you vibecode your way to a fragile, poorly understood project. It will not force you to learn.



For those who want to truly learn, AI is not the perfect answer key. It can be a catalyst for curiosity, but only if you have the discipline to question it, the diligence to research its claims, and the courage to turn it off and think for yourself. I approached AI to learn how to build a voxel engine, and I succeeded. The most important thing I built, however, was not an engine or a prize-winning algorithm, but a workflow that prioritizes human understanding over machine output.