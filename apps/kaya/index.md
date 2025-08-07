---
title: "Kaya"
date: 2021-11-22
layout: page
categories: [apps]
image: assets/img/kaya-icon.png
---

[Kaya](https://codeberg.org/leaf-node/kaya) is a Bash front end for
[restic](https://github.com/restic/restic), a modern incremental backup
solution written in Go. Kaya provides centralized backup functionality via SSH,
similar to "pull" mode backups, but with most of the heavy lifting being done
by each client. Kaya makes use of restic's
[rest-server](https://github.com/restic/rest-server) in append-only mode, so in
theory, backed up machines can't delete their past backups, nor see backups for
other machines.
