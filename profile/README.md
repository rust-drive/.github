# Rustdrive

The goal of this project is to create a cloud that is easy to use for users

There are many cloud services you can host, but most users are confused by the variety of options available to them. To view file details, there are several tabs and options in Nextcloud. So the aim of this project is to create a cloud that makes cloud services easier. It'll probably just be for learning purposes, but we'll never know...

|![Static Badge](https://img.shields.io/badge/with_love-orange?style=for-the-badge&logo=rust)|![Static Badge](https://img.shields.io/badge/with_passion-blue?style=for-the-badge&logo=docker&logoColor=white)|![Static Badge](https://img.shields.io/badge/with_patience-yellow?style=for-the-badge&logo=javascript&logoColor=white)|![Static Badge](https://img.shields.io/badge/with_magic-purple?style=for-the-badge&logo=bootstrap&logoColor=white)|

|---------------------|--------------------|--------------------|---------------------|

## Authors

- [@Soraxem](https://github.com/Soraxem)

## Structure

```mermaid
graph TD
  user --> frontend
  apps --> frontend
  configuration --> frontend

  frontend --> backend
  backend --> database
  backend --> files

```
