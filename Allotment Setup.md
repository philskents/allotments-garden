---
type: note
description: A basic note structure with no additional properties other than status and tags and links
---
---

**Links**: [[Home]]

---

# Allotment setup
## TLDR
### New allotments
- Create a new empty git repository on your git server
- Add it as a submodule to your parent git repository
- Set the tracking branch for your submodule

## New Allotments
For new Allotments you start at your git server (GitHub for me) and create a new git repository. Add a single file so we have something to validate with (delete it after the setup is complete). Once that is created you can go ahead and add it to your main repository by running the following command in the root of your vault.

`git submodule add git@REMOTE_URL:/path/to/git/repos/allotment.git path/in/vault`

