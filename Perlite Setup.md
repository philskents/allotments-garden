---
type: note
description: A basic note structure with no additional properties other than status and tags and links
---

---

**Links**: [[Home]]

---

# Confiuring a Publishing Workflow
The [Perlite](https://github.com/secure-77/Perlite) setup is a multi-part workflow that will deliver a Perlite Docker container hosting your Allotments and ready to push to a contaner host of your choice. I am using GitHub Actions to orchestrate this workflow.

### Repo setup


We are creating (yet another) git repository which will host the code and submodules required to build our published site. Once you have creaated the folder on your git server clone it to yor local machine.

`git clone git@REMOTE_URL:/path/to/git/repos/allotment-manager.git`

Create a folder in the root called allotments and link your allotments as submodules into that folder.

`git submodule add git@REMOTE_URL:/path/to/git/repos/allotment.git allotments/allotment-name`

I also forked the Perlite repo and added it as a  submodule as well as we will need to make some changes to it. The code can be found in this [repo](https://github.com/philskents/Perlite) including the changes but to summarize:

- Modified the dockerfiles so both the web and the app containers get a full copy of the static files (Lightsail Container service does not support shared volumes)
- Modified the dockerfiles so the markdown is copied into the containers (again, no volumes)
- Modified the nginx config to use localhost instead of the app container name (Lightsail doesnt provide container name resolution)
- Modified the blog link to point to my blog

## GitHub Actions

