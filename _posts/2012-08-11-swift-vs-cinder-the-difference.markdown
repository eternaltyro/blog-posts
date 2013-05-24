---
layout: post
title: "Swift vs. Cinder: The difference"
date: 2012-08-11 01:53
comments: true
categories: 
---

Openstack uses two kinds of storage entities to store stuff. One is Cinder (previously nova-volume) that provides a block storage service for Nova instances. Swift is a standalone object store. Swift is distributed, massively scalable and eventually consistent.

Swift is:
---
* An object store - Objects are just data blobs.
* API Based - All operations are undertaken using RESTful API calls.
* Distributed - No central point of failure and objects are replicated heavily.
* Massively scalable - It can scale to petabytes of data and can easily handle backend scaling out.

swift is not:
---
* Swift is not a block storage - It is a flat storage and there is no concept of blocks.
* Swift is not a file storage
* Swift is not mountable
* You can't mkfs Swift

