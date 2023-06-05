# Deploy apps on the router like a pro with app manager on IOS XR

## Introduction

Welcome to DEVWKS-2125! This is your guide to developing and deploying your own docker applications for Cisco routers running IOS-XR software.

In this workshop you will learn about IOS-XR's application hosting features. We will package an open-source DNS server's docker image (Ubuntu-based bind9) into an IOS-XR supported ```.rpm``` package using appmgr build scripts (https://github.com/ios-xr/xr-appmgr-build).

After creating our ```.rpm``` packages, we will login to the router to install and run our application using IOS-XR appmgr CLI commands. While on the router shell, we will learn about other appmgr CLI commands to monitor running applications and installed packages.

Finally, we will test our application by trying simple DNS requests from a client connected to the router. We will use these DNS requests to discsuss how packets make their way to and from Third Party Applications on IOS-XR. 

Bonus content includes instructions to make your application VRF aware and guidelines for running telemetry applications on the router!


## General Guidelines

- Please feel free to ask any workshop-related questions during the session. For general IOS-XR application hosting related queries, meet me after the session to schedule time for a detailed discussion.

- You will use a Cisco anyconnect VPN to connect you to the workshop sandbox environment. You can find instructions to connect to this VPN at your desk and on the WebEx. The WebEx space with these details will be accessible through the workshop laptop.

- Environment: You are going to be using Virtual XR routers (running virtualized Cisco 8000 instances) and Centos7 Devbox VMs (for building images). You will use ssh to connect to these devices whenver needed. Again, ssh connectivity details will be on your desk or accessbile through WebEx on the workshop laptop.

- I will use the "DNZ Workshop 05" WebEx space to broadcast any instructions/commands/messages during this session. Your workshop laptop should be a part of this space.