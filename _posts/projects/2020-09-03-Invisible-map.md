---
title: "Invisible Map - IOS App Development"
permalink: /project/project_invisible/
categories:
  - Project
tags:
  - Accessibility
  - Swift
  - iOS
  - AR
toc: true
toc_label: "Table of Contents"
toc_icon: "heart"
toc_sticky: true

gallery:
  - image_path: /assets/images/invisible/1.jpg
    url: /assets/images/invisible/1.jpg
  - image_path: /assets/images/invisible/2.jpg
    url: /assets/images/invisible/2.jpg
  - image_path: /assets/images/invisible/3.jpg
    url: /assets/images/invisible/3.jpg
  - image_path: /assets/images/invisible/4.jpg
    url: /assets/images/invisible/4.jpg
  - image_path: /assets/images/invisible/5.jpg
    url: /assets/images/invisible/5.jpg
  - image_path: /assets/images/invisible/6.jpg
    url: /assets/images/invisible/6.jpg
  - image_path: /assets/images/invisible/7.jpg
    url: /assets/images/invisible/7.jpg
---

## Introduction

The invisible map project is an iOS accessibility app created by the OCCaM (Olin College Crowdsourcing and Machine Learning) Lab, that enables blind people to navigate inside buildings without using external devices other than their phones. There have been different approaches people tried to help blind people navigate indoors - some of them created high accuracy through using external devices, but the fact that they have to use external devices becomes a great limitation once it is related to accessibility. 

The basic idea behind the invisible map is that there will be two different types of stakeholders: people who will set up the map for buildings, and one who will use the app to navigate. Once the map is created by the first group of users, the other group of users will be able to navigate just by holding their phone in their hand. This method has a great limitation too - the app will be useless if there is no pre-built map for the buildings. The idea behind the app is very impressive, where once the map is created, there comes great convenience for blind users. However, a major concern for our team was thinking of how will we be able to have people set up the map of their businesses. In other words, the app should have a big user group to properly function. The question is currently unsolved, but we are trying on multiple different approaches. 

## Summary

I worked on designing and creating UI/UX for the early version of the app during the summer of 2020. The process was mostly designing the UI and testing the prototypes so that we can test on different approaches. The current version of the app is very different from what is done during summer 2020 because people have been building upon the research after that, but the design choices were made based on the observation made during that period.

The app uses April tags and Apple ARkit to initialize and track the correct position of the user. We used AR to correctly recognize the tags and position of the user in real-time, and this was important since we wanted to get the exact position of the user regardless of the initial tag's angle/position in the camera, and the main user of the app was blind people. Since the app uses the tag as a start point to draw the map on augmented reality (AR), having a wrong start point can mess up the result. 

One part I worked on was creating a recording system that will be used by the users who want to set up an invisible map for their business. The app will be able to start recording once an April tag was detected, and the map will be recorded according to the route the user traveled. The route data will be cleaned up by the app in form of .json, sent to firebase, and the 3D visualization of the invisible map will be created by a running server that those the computation. The finished map will be saved back in the firebase, where the app will be able to load the data in real-time once the same tag was detected when navigating. 

Saving a specific location was an important function that I also worked on. Navigating inside a building is good, but you want the user to know where you are navigating toward. By setting up important locations, the map not only tells you which route to follow but also tells you where you are going. Each location was saved relative to the position of the initial April tag, and the user could manage the list of locations and create/modify/delete locations on a map.

There was some limitation on the app when it was under development last summer. The biggest issue was the accuracy of the map. The map is amazingly accurate in the scope of how difficult it is to set up a map, but it was not good enough to have a blind person navigate through just relying on the map itself. Sometimes it had an error between a foot to a yard, which can be crucial if it is around the wall/staircase. Currently, the team is working on improving the 3D visualization model of the map and also trying to use extra April tags that will automatically adjust the error once the phone detects it. 

## Progress

{% include gallery id="gallery" %}

## Result

From the project, I learned:

- Learn the basics of UI/UX such as creating a prototype with Figma, considering user group, and multiple iterations.

- How to develop an iOS app using Swift

- Working as a team to create an app, and collaborating with different teams (ex. The server team) to complete a task.

- Understand and research the need for accessibility in technologies.