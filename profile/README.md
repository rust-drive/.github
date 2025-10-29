# Rustdrive

![Static Badge](https://img.shields.io/badge/with_love-orange?style=for-the-badge&logo=rust)
![Static Badge](https://img.shields.io/badge/with_passion-blue?style=for-the-badge&logo=docker&logoColor=white)
![Static Badge](https://img.shields.io/badge/with_patience-yellow?style=for-the-badge&logo=javascript&logoColor=white)
![Static Badge](https://img.shields.io/badge/with_magic-purple?style=for-the-badge&logo=bootstrap&logoColor=white)

This project with aims to create a intuitive cloud.

I host a nextcloud, but some of my clients are confused over the loads of options they have. Just to look at a files details there are multible tabs and options. So i decided that it is time again for a Project. It propably only will be for learning purposes, but you will never know..

## Structure

The Server is built like a static webserver. Acess control is built with json files. The API is application agnostic, it just delivers a file-storage backend for the Applications.

```mermaid
graph TD
  user --> wrapper
  
  server --> files
  server --> apps
  server --> wrapper
  wrapper --> apps
```

## Federation

A big goal of this project is smooth and intuitive federation. A server stores users and guests. Guests are users from other servers, that need credentials on this server. 

```mermaid
graph TD
  subgraph server-1
    users-1
    guests-1
  end

  subgraph server-2
    users-2
    guests-2
  end

  users-1 --> guests-2
  users-2 --> guests-1

```
