---
type: note
description: A basic note structure with no additional properties other than status and tags and links
---

---

**Links**: [[Home]]

---

# Confiuring a Publishing Workflow
The [Perlite](https://github.com/secure-77/Perlite) setup is a multi-part workflow that will deliver a Perlite Docker container hosting your Allotments and ready to push to a contaner host of your choice. I am using GitHub Actions to orchestrate this workflow.

We are creating (yet another) git repository which will host the code and submodules required to build our published site. Once you have creaated the folder on your git server clone it to yor local machine.

`git clone git@REMOTE_URL:/path/to/git/repos/allotment-manager.git`

Create a folder in the root called allotments and link your allotments as submodules into that folder.

`git submodule add git@REMOTE_URL:/path/to/git/repos/allotment.git allotments/allotment-name`