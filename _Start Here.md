---
tags: digital-garden allotments
---

# Introduction

## Summary

This is my plan to provide an alteranative to [Obsidian Publish](https://obsidian.md/publish) that allows more granular publishing for my Digital Garden and more choice in how you publish and what platforms you publish to.

Obsidian git now apparently supports git submodules and that is a game changer for this project. I am going to refer to this methodology as Allotments purely as a throwback to [this wonderful British tradition](https://en.wikipedia.org/wiki/Allotment_(gardening)) which was [solarpunk](https://builtin.com/greentech/solarpunk) before it was cool!

My new strategy is as follows:

- A single Obsidian vault backed up and synchronized using git will form the core of my Obsidian setup
- This will require some specific vault configurations to support Allotments (see [[Vault Setup]])
- Each Allotment will then as a git submodule (see [[Allotment Setup]])

At this point you now have a bunch of markdown and associated attachments that you can host in a variety of ways stored away from your main vault. I decided to use [Perlite](https://github.com/secure-77/Perlite) for this as it seems to be the best option right now to handle Obsidian's markdown eccentricities.