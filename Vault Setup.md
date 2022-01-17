---
type: note digital-garden
description: Vault setup for an allotments style publishing method
---

---

**Links**: [[_Start Here]]

---

# Vault setup for Allotments
---
## TLDR
- You need a vault that uses obsidian-git for backup/sync
- Sort content for publishing into one or more folders
- Configure images and attachments to be stored with the current file

---

## Setup
Firstly you heed to have an Obsidian vault setup and configured to use [obsidian-git](https://github.com/denolehov/obsidian-git) for backup and sync.

The core premise of Allotments is that, within your digital garden, any shared content exists within one or more specific folders. For example this particular body of work exists in my vault as ```VAULT_ROOT/🗂 Projects/Digital Garden Publishing``` . I also want to use this metodology for publishing my #PaintSlam22 progress so content related to that will live in ```VAULT_ROOT/🗂 Projects/Paint Slam 22``` and so on.

To ensure each allotment can be as self contained as possible we need to ensure all artifacts pertaining to that allotment are contained within that file strucure. Obsidian allows you to change where images and attachments are stored in relation to a page and how they are linked. In ```Settings -> Options -> Files & Links -> Default location for new attachments``` you can select either option that stores them in relation to the current file (I prefer a subfolder for ease of organization) and then change how they are linked by changing ```Settings -> Options -> Files & Links -> New link format```  to `Relative path to file`

![[attachments/Screen Shot 2022-01-13 at 14.32.54.png]]