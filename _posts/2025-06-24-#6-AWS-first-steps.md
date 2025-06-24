---
layout: post
category: "AWS"
subtitle: "Just trying something new here .. again :)"
author: "Tino"
---
It was quite an amazing day to be honest, so let's see what happened!

As I have worked in modern IT environments for quite a while, I always wondered about how the cloud service providers actually work.
Coming from a world where I deployed docker containers in docker swarm on RHEL servers, 
I had some rough ideas - but never had the time to explore by myself. 
Apart from watching random youtube videos about it. 

So with Claude (Sonnet) next to me I began to explore what it feels like to get my hands dirty on AWS.

First of all: setting a goal
To not only explore it theoretically I wanted it to be tangible, so I needed a project.
This was fairly easy because asking Claude to help me out gave me a nice route that I could explore.
So the task was to get a small react app (notetaking app) to run in AWS, touching multiple services (we come to this later).

Starting with creating an AWS account and configured the CLI (just to have more fun later in their webui ..  nyway...).
Touching the first service already: Lambda! A quick hello world later, it was already exposed using the API Gateway.
For the notes app I needed a table, so I ended up in DynamoDB and set up the correct IAM properties so that Lambda was able to write something in there.
I instructed Claude to improve the UI of the notes app a little, until I was happy with the design and therefore ready to deploy it.
<p style="text-align: center;"><img src="{{ site.baseurl }}/images/postpics/aws-first-steps.png" alt="Meditation" style="width: 400px;"/></p>

In between I got some automation taste by setting up Amplify so that I could just push my code from VS Code to github and this was then just grabbed
and deployed to a S3 bucket.
Since I had some initial trouble with my API Claude helped me out with fitting my Lambda functions with some code so I would also see some metrics and logs in Cloudwatch.

All in all it was a very fun journey!




 
