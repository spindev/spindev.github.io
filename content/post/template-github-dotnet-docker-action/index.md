+++
title = "Template for creating custom GitHub .NET Docker Actions"
date = 2024-04-26T15:38:30+08:00
header_img = ""
toc = false
tags = ["GitHub", "GitHub Actions", ".NET", "Docker"]
categories = ["GitHub"]

# series = ["Themes Guide"]

+++

Recently I had to solve a more complex problem for a customer. When I encounter more complex problems in my daily work that can't be solved with a few Bash or Powershell commands, I use my favourite language C# and the .NET framework. I am a big fan of the .NET framework and have worked with it for most of my IT career. Situations like this also help me to familiarise myself with the latest developments and to get to know the new stuff and try out new functions.

In this particular case, a GitHub Actions workflow has to be created, which makes various API queries and processes the data further. As part of my work as an accredited GitHub Trainer, I am familiar with the three types of GitHub Actions and so this time the choice fell on a Docker Action based on .NET. But where is the best place to start, how to pass parameters and how to provide values as outputs? With the help of Google, I came across the following guide, which was a good starting point, but too overloaded for me:

https://learn.microsoft.com/en-us/dotnet/devops/create-dotnet-github-action

However, I wanted to have a basic & lean template on GitHub that provides me with the required stuff for a GitHub .NET Docker Action and can serve as a basis for later tasks. Open source, of course, and therefore usable for everyone else.

No sooner said than done. The repository contains:

- a [action.yml](https://github.com/spindev/dotnet-docker-action/blob/main/action.yml) file for the definition of the GitHub Action
- the [.NET Docker Action project](https://github.com/spindev/dotnet-docker-action/tree/main/DotNet.DockerAction)
- a [Dockerfile](https://github.com/spindev/dotnet-docker-action/blob/main/Dockerfile) to dockerize the .NET project
- a [testing workflow](https://github.com/spindev/dotnet-docker-action/blob/main/.github/workflows/test.yml), because we are always following the DevOps principles, right?

You can find the template for a GitHub .NET Docker Action here:

https://github.com/spindev/dotnet-docker-action

Simply use the green button ‘Use this template’ and create your own GitHub .NET Docker Action. Have fun with it. If you are missing something, feel free to create a pull request.
