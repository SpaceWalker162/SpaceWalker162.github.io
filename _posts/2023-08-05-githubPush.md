---
title: Push to github
date: 2023-08-05
permalink: /posts/2023/pghjlew
excerpt_separator: <!--more-->
toc: true
tags:
  - web-dev
---
Problems I encountered when pushing to github.
<!--more-->

## network connection
error message:

        Failed to connect to github.com port 443: Timed out

The solution is to use proxy:

        git config --global http.proxy http://127.0.0.1:7890
        git config --global https.proxy http://127.0.0.1:7890

## HTTPS connection
account password for authentication is no longer supported. To push via https, use a personal access token in place of password when asked to type in. Personal access token can be generated at the website through `settings → developers settings → Personal access tokens (classic) → generate new token`.

## SSH connection
follow the procedure described at https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

