# Complete Docker Course - From BEGINNER to PRO! (Learn Containers)
#https://www.youtube.com/watch?v=RqTEHSBrYFw
#https://github.com/sidpalas/devops-directive-docker-course

![alt text](image.png)

## 1. History and Motivation
virtualisation techniques come from: bare metal
then: VMs
now: containers

A docker container is a ligthweight, standalone, executable package of software that includes everything needed to run an application.

Container image is an artifcat with all the dependencies in it. While a container is what you run from that image.
From Object-Oriented programming perspective: image is the class and the container itself is an instance of that class.

Few early players, Docker one of them, but instead of having the container technology vary slightly across them, there is the Open Container Initiative (OCI) pushing for open industry standards around container formats and runtimes. Collab of Google, Dell, VMWare, Docker,... Three things: 1. Runtime specification (how you take that image and run it in a container in adherence to the image), 2. Image specification (metadata, what should be included in the image and the format so a serialisable file system), and 3. Distribution specification (registries, pushing and pulling images).

Docker has a specific implementation of these OCI standards.

The evolution of virtualisation:
![Bare metal virtualisation and the downsides](image-3.png)

![Virtual machines virtualisation](image-4.png)

Hypervisor is some combo of software and hardware that allows us to carve up the physical resources into isolated smaller pools which we can then use to install our system on.
Type 1: no underlying OS. Beneficial: no performance sacrifice since everything runs directly on the hardware. E.g.: AWS Nitro, VMware Sphere.
Type 2: Virtual Box, classic on your own machine at home.

![Virtual machines characteristics](image-5.png)
big advantage over bare metal: fast provisioning and decommissioning (look at cloud providers).

![Containers virtualisation](image-6.png)

key difference VMs and containers: VMs run their own copy of the Linux kernel. This course will only treat Linux containers. While Linux containers are sharing their Linux kernel with the host operating system.

![Containers characteristics](image-7.png)
Small blast radius, but not quite as much as a virtual machine.




## 2. Technology overview

### Containers
### Docker



## 3. Installation/Set-up & Hello World



## 4. Using 3rd party containeres


## 5. Demo Application
![alt text](image-1.png)

## 6. Building container images

### Dockerfile basics
### Dockerfile optimisation
### Buildx + multi-architecture


## 7. Container registries


## 8. Running containers


## 9. Container security


## 10. Interacting with Docker objects


## 11. Development workflow


## 12. Deploying containers



