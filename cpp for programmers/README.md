# C++ For Programmers

[https://www.udacity.com/course/c-for-programmers--ud210](https://www.udacity.com/course/c-for-programmers--ud210)

## Setup Guide

### Docker

Install Docker on your machine: [https://www.docker.com/get-started](https://www.docker.com/get-started)

After the installation, go to preferences, and set the number of CPUs to the maximum capacity of your computer.

```bash
docker build -f Dockerfile -t udacity/cpp . # builds the image
docker run -it --rm -v "$(pwd)":/udacity:delegated -w /udacity --name Udacity-CPP udacity/cpp # runs the container
docker exec -it Udacity-CPP ash # go inside a running container
docker kill Udacity-CPP # kills the container
```

## Compiling

To compile files, use the command bellow:

```bash
clang++ -Wall -std=c++17 <input_file>.cpp -o <output_file>.out
```

> The .out exntesion is not mandatory for the output,  
but it's there because it's ignored on this repo

## Styleguide

I will follow the [Google C++ styleguide](https://google.github.io/styleguide/cppguide.html) for this repository.
