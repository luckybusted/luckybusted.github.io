---
layout: post
title: Make Alexa write JSON files
category: Alexa

excerpt: How I Made Alexa write Json files and save them to a Server.

---

# Make Alexa write JSON files

The idea was to save the JSON Request files that came out of the AVS (Alexa Voice Service) on a regular ftp sever so any device/service can get them without give Alexa the permission to go beyond firewalls etc.

It will look something like this: 

![Alexa to S3 to RasPi workflow](/assets/Alexa-Json-workflow-1.png)

This may be a hint: https://foobar123.com/serverless-save-a-file-in-s3-using-aws-lamdba-d3f087880dd2

So first of all we create a simple alexa skill and test it. If everything went fine we will recieve a respond, that everything is allright.

So now we can create a AWS S3 bucket where we will store our files.