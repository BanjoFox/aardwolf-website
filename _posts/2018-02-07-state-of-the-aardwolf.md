---
title: State of the Aardwolf
date: 2018-02-07 10:24
---
## Current state of the Aardwolf code
- The server compiles
- The Master branch, which uses Handlebars.rs for the web templates will render okay, and work for testing logins
- Logins work, but the auth-token is sent to STDOUT so I literally have to copy/paste it into a browser to authenticate new users
- We are migrating to Tera for templates, but the language files are not -yet- in the correct context which causes a 500 error because Rocket/Tera is trying to populate the `{{ strings }}`

### High Priority TODO's
- Bring the language files from /lang/*.toml into the correct context (fixing Tera runtime issue)
- Configure something for e-mailing the auth-tokens

### Alpha-release (MVP) Targets
- Develop functionality for a single-instance "shoutbox-like" posting
- Basic federation between two servers 

***
