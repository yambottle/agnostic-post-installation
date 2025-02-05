# agnostic-post-installation
Normalize post OS installation setup automation

Problem: For a solo dev, everytime setting up a new laptop or reinstall the OS or switching from Linux to Mac to Win, it takes a day or two to setup a new environment that is slightly different than what it used to feel like. Mostly because there is an application that you forgot to install or certain configuration wasn't kept as previously did. For a team, this is a consistent base standard initial dev env that everyone could start with. Seems like a configuration management problem or a common IT's problem, but I didn't find such tool that ready to use.

- Similar solutions:
  - https://github.com/snwh/ubuntu-post-install
  - https://github.com/naushadS/dev-setup
  - https://github.com/TerrorSquad/ansible-post-installation
- Ideal solution:
  - companies are more and more using remote dev pod/instance or IDP, this project should be lightweight
  - have a set of common software can be installed by user roles[dev, data, devops, all]
  - supports linux, mac and win + wsl
  - supports localhost or broadcast more laptops
  - supports exporting existing env, then can be reinstalled/reconfigured later, possibly across OS
  - expect users of this tool or people been served by this tool would be very opinionated about their own dev env, this tool should be very easily to be forked then customized
- Minimal solution:
  - have a set of common software can be installed by user roles[dev, data, devops, all]
  - supports linux
  - supports localhost
- Reference: 
  - https://github.com/jondot/awesome-devenv
  - https://github.com/TerrorSquad/ansible-post-installation

```
## system update

## system lib
# build-essentials
# net-tools
# gzip, tar
# tree
# common dev lib


## common tools
# gnome tweaks
# terminator
# terminator theme
# chrome
# slack
# zoom
# vscode
# vscode workspace
# spotify
# yubikey manager

## dev tools
## dotfiles: https://github.com/tomnomnom/dotfiles
# .bashrc
# .alias
# vim
# .vimrc
# git
# github cli
# aws cli
# mamba
# poetry
# npm
# go
# rust
# mysql/mariadb
# percona-toolkit
# docker desktop
# postman
# yq
# jq

## devops tools
# rancher desktop
# kops
# k3s
# k3d
# kubectl
# kustomize
# helm
# terraform
# packer
# s3fs
# act - local run github actions
# ansible

## data tools
# nvidia driver
# cuda toolkit
# cuda container runtime

## generate user docs after installation
# what installed
# what can be customized
# what's next
```
