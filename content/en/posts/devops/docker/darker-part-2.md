---
title: Learn Docker in 5 parts (Part 2 - Basic Commands)
date: 2021-04-26T12:12:06+09:00
description: Docker accelerates how you build, share and run modern applications without worrying about environment.
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

## Welcome

In the previous article, I already explained what Docker is, general concepts, and purpose of Docker. In this second article, I will describe how to use its most essential basic commands.

Here the links to previous article: <a href="https://blog.kimleang.cyou/posts/devops/docker/docker-part-1/" target="_blank">Docker Part 1: General Concepts</a>

You're required to Docker installed and running in your machine. Docker installation document is very straight forward. You can have it installed in your Mac, Windows, and Linux. [Docker Install Docs](https://docs.docker.com/get-docker/).

It may be very tedious for waiting its downloading and installing. But, there's an online alterantive, where you can use Docker without installing. It's called [Play-With-Docker](https://labs.play-with-docker.com/).
**Caution**: Play-With-Docker, It should be used for learning purpose only. Don't provide any sensative data such as password, etc. And note that 1 session is only 4 hours, after that everything will be wiped out completely.

## Never forget to say Hello World

A **Hello World** program is typically one of the simplest programs for every computer languages. So, don't forget it, open your terminal, let's say **Hello World**.

```bash
docker run hello-world
```

You'll able to see something like this:

```
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
1b930d010525: Pull complete
Digest: sha256:2557e3c07ed1e38f26eXXXXXX3ed943586f744621577a99efb77324b0fe535
Status: Downloaded newer image for hello-world:latest
Hello from Docker!
This message shows that your installation appears to be working correctly.
To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.
To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash
Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/
For more examples and ideas, visit:
 https://docs.docker.com/get-started/
```

So, it's working. In the command above, you'll notice 3 parts of it.
- **docker**: a prefix command that use to run every docker commands.
- **run**: a command that first *creates* a container and then *starts* it using the specified image.
- **hello-world**: an image name than can be used to create containers. Can be found on [Docker Hub](https://hub.docker.com/).

After run the command above, you will see log from it. One interesting line is: ***Unable to find image 'hello-world:latest' locally, Pulling from library/hello-world***.
This line indicates us that there's no image in your local computer, so it has to be pulled from Docker Hub, where all images are stored, and work with it. However, once you complete pulling it, next time you run from the same image, it will find and use your local image.