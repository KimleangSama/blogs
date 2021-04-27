---
title: Learn Docker in 5 parts (Part 1 - General Concepts)
date: 2021-04-26T12:00:06+09:00
description: Sample article showcasing basic Markdown syntax and formatting for HTML elements.
draft: false
hideToc: false
enableToc: true
enableTocContent: false
author: Kimleang
authorEmoji: 🚢
tags:
- devops
- docker
- container
categories:
- devops
series:
- Docker Guide
image: /images/posts/docker/docker-logo.png
---

![Docker Logo](/images/posts/docker/docker-logo.png)

## Prerequisites

The readers should be familiar with the basic concepts of Linux OS whether it's Ubuntu, CentOS or others.

If you can afford it, go get this best course about Docker [Docker Mastery: The Complete Toolset From a Docker Captian](https://www.udemy.com/course/docker-mastery) created by **Bret Fisher**.

## Introduction

Docker is a container management service. The keywords of Docker are **develop**, **ship**, and **run** anywhere. The main goal of Docker is to help developers to easily develop applications, ship them into containers which can then be deployed anywhere.

## Why do we need Docker?

Have you ever heard or seen meme all about "It works on my machine."??

![It-Works-On-My-Machine](/images/posts/docker/work-on-my-machine.jpg "It-Works-On-My-Machine")

Let's flash back how we used to develop and deploy applications in the old days.

Back then, we needed to install all the necessary dependencies in our local machine. The database (MySQL, Postgres), the web server (Apache, Tomcat, Nginx), the build tools (Maven, Gradle, NodeJS) and the other required software. Once we installed everything, we could start coding our applications.

After months of implement our application, we would have our application ready to be deployed.

##### &nbsp;&nbsp; And here is where the problems started...

Do you remember we had to install all the dependencies in our local machine? Now we had to do the same in the server and make sure that everything worked flawlessly as well as your local machine. Since the server environment was usually different from our local machine, which would lead to consuming several hours in configuring every single detail.

![Work-Fined-In-Dev](/images/posts/docker/work-fined.jpg "Work-Fined-In-My-Machine")

We could use other solutions like **Vagrant**, but that is in other topics.

##### &nbsp;&nbsp; And Docker was born

Let’s check the definition of what a container is on the Docker official page

> A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

Not clear, right? Okay, let's take a look of this diagram below:

![Docker Diagram](/images/posts/docker/docker-diagram.png "Docker Diagram")

Here we have several apps running; each of them has a single context, which does not share it with any other app. Also, all the apps are running on top of the Docker Engine, which is the layer responsible for providing an interface from the apps to the OS and vice-versa. By the word "interface" means a point where two systems meet and interact.

## Docker Containers

Containers are instances that wrap applications along with required dependencies. Containers themselves are exportable, destroyable, and immuntable. You can think of a container like a little box running you app. That small box can be running anywhere no matter it is in your local machine, production server. Only thing you have to do is wrapping your apps in the box and moving the box to the production server.

## Docker Images

A Docker Image is a container's template which can be used to create Docker Containers. Using OOP concept, we can think an image as a "class" where containers as "objects". A class creates Objects, and Objects created from a Class.

We aren't gonna talk in depth about Docker Images and Containers here yet. But we will discuss in the next topic. **Stay Tuned.**

## In Summary

Docker is a tool where you can develop, build, and ship your applications easily without caring about the environment between your local machine to other machines such as testing server and production server.

Docker also guarantees that your app will 100% work everywhere no matter which environment it's in.

This is just a breif introduction about Docker. And you still can learn about it from other website, search for it. Anyway, don't forget to ~~subscribe~~ oops, to download Docker from official website in your machine. 

Here official website: [Docker](https://www.docker.com/products/docker-desktop)