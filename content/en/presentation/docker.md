---
title: "Docker Pt"
date: 2019-10-30T20:48:10+09:00
description: "Docker Slide Presentation"
tags:
- docker
series:
- DevOps
categories:
- devops
plugins:
- zoom

image: /images/presentation/presentation.png

highlightTheme: monokai
revealTheme: black
revealBackgroundColor: "" # #fff or rgba() or hsl()
revealBackgroundImage: "" # /images/myImage.png   <= static folder path
revealBackgroundPosition: "" # left top, left center, left bottom, right top, right center ...
revealBackgroundRepeat: "" # repeat, repeat-x, repeat-y, no-repeat, inherit
revealBackgroundOpacity: "" # 0~1
revealBackgroundVideo: "" # /videos/myVideo.mp4 <= static folder path, A single video source, or a comma separated list of video sources.
revealBackgroundVideoLoop: false # true, false
revealBackgroundVideoMuted: false # true, false
revealBackgroundSize: "" # cover, contain, ...
reveal: 
  - main:    
    - sub: 
      - |
        # Docker
        ### The world’s famous container management service.
        
  - main:    
      - sub: 
        - |
          ## I. Introduction
          Do you know the famous phrase "it works on my machine"?
      - sub:
        - |
          This phrase is related to the problem that your application only work when you're developing it in your local machine (Computer).
      - sub:
        - |
          If you never experienced this, you might say "Really? Ohh come on, If it works on my computer, it should work on other computer as well". 
          
          Is there any problems with their computer? 
          
          The answer is "Maybe".
      - sub:
        - |
          If you develop a NodeJS app, you may likely use the latest version of Node. 
          
          You just hit ```npm start```, then bomb, it starts. 
          
          And then you copy your code to your friends via a **USB flash drive** to paste and run it. 
          
          You expect to impress your friends with your apps, until it...
      - sub:
        - |
          Error: The module '/some_modules' was compiled against a different NodeJS version using NODE_MODULE_VERSION X. This version of NodeJS requires NODE_MODULE_VERSION Y.
      - sub:
        - |
          It's because your friends are using NodeJS older version than yours. 
          
          Because of that they don't see a sh*t in your apps. 
          
          So the phrash "It works on my machine." is really work on your machine. 
          
          And...

      - sub:
        - |
          Are there any ways to solve this problem??
          Yes, there are. It can get its a** kicked by using **Docker**.

  - main:    
      - sub: 
        - |
          > Docker is a tool designed to make it easier to create, build, deploy, and run applicatiosn by using containers, and eliminate the phrase "It works on my machine".
  
  - main:    
      - sub: 
        - |
          ## II. Benifits of Docker
      - sub:
        - |
          #### 1. Constistent and Isolated Environment
          Using Docker Containers to isolate your app from the environment and other apps. 
          
          Also, containers are exportable, destroyable, and immutable that make them easy to work with.

      - sub:
        - |
          #### 2. Scalability
          You can quickly create new containers if demand for your applications requires them. 
          
          When using multiple containers you can take advantage of a range of container management options.
      
      - sub:
        - |
          #### 3. Version Control
          The Docker Image lets us change and manage the version of our applications. 

          This is called "tags" where you can tag different version of your application and publish to Docker Hub.

      - sub:
        - |
          #### 4. Security
          The applications on containers are completely separated from each other, to ensure the full control on the management: a Docker container cannot see the running processes inside another container.

  - main:
    - sub: 
      - |
        # To be continue...
        
  - main:
    - sub: 
      - |
        # Powered by Reveal.js
        ### A framework for easily creating beautiful presentations using HTML.
        - [Check out the live demo](https://revealjs.com/#/)
---
