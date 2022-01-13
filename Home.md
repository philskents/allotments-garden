---
type: note digital-garden
description: Design and build a method whereby I can publish multiple "digital gardens" to public hosting from a single Obsidian Vault.
published: true
---
# Introduction
## Summary
This is my plan to provide an alteranative to [Obsidian Publish](https://obsidian.md/publish) that allows more granular publishing and more choice in how you publish and what platforms you publish to.

Obsidian git now apparently supports git submodules and that is a game changer for this project. I am going to refer to this methodology as Allotments purely as a throwback to [this wonderful British tradition](https://en.wikipedia.org/wiki/Allotment_(gardening)) which was [solarpunk](https://builtin.com/greentech/solarpunk) before it was cool!

My new strategy is as follows:

- A single Obsidian vault backed up and synchronized using git will form the core of my Obsidian setup
- This will require some specific [[Vault Setup|vault configurations]] to support Allotments
- Each Allotment will then become a git submodule
