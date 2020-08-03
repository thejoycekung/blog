---
layout: post
title: Building a Guestbook in Flask
date: 2020-08-02
---

[link to repo](https://github.com/thejoycekung/tinkering/tree/master/hello_world)

When I first started this project I didn't really know where I was going. I started by following Miguel Grinberg's [Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world) which guides you through creating a "microblog" app (somewhat similar to Twitter). I eventually decided against this, as my end goal here wasn't to learn more about Flask, it was to have something that:

1. Would need to be deployed online, somehow
2. Would need a separate service (e.g. a database) so that I could have practice hooking up different things together

Eventually, after some research, I settled on the idea of a guestbook. It was close enough to the idea of the microblog (but without the additional complexity of having users/logins) and popular enough that if I inevitably got stuck, I'd be able to find help somewhere.

Other than the major difference of making a guestbook, I also differed from the Mega Tutorial because I neglected to fix how time is displayed, and I didn't put nearly as much effort into how the site looks. The main goal was how to set it up and get it running.

A list of resources I also read while making it (other than the Mega Tutorial linked above):

* https://github.com/KevinJones/flask-guestbook-example
* https://medium.com/@mudasiryounas/kubernetes-docker-flask-postgres-sqlalchemy-gunicorn-deploy-your-flask-application-on-57431c8cbd9f

## Things that went well

I've gotten way more comfortable with Python in the past year (and a half or so). I didn't have to write that much Python, but writing it has gotten easier and easier ever since I've tried using it as my main interviewing language and practiced it more and more.  
My goal is to take that knowledge of how I got better at Python and use that with Go (soon!).

Another thing I've done before and felt familiar - the HTML templates. Writing the templates felt like something from a forgotten era - I started coding when I wrote Tumblr themes in around 2014, so those `{ }` felt pretty damn familiar.

This was my first time using a Python virtual environment and creating a `requirements.txt` - and it all went over smoothly! Thank god.

This was also my first time writing my own Dockerfile! Overall it went pretty smoothly and I'm pretty happy I had multiple sources to consider (from the tutorials I looked at). I also recently learned about [the difference between `ENTRYPOINT`, `CMD`, and `RUN`](https://dominikbraun.io/blog/docker/dockerfile-run-vs-cmd-vs-entrypoint/), which was super helpful in writing it!

## Things that I can improve on

I definitely wish I felt more comfortable with Terraform. The Terraform file that I used was lifted (almost? I can't tell) from Artemmkin's IaaC tutorial and I wish I tried writing my own (even if it is super simple, just like that one!). I think I'm going to delve a bit more into the Terraform tutorials available on their website and see whether that can help.

I also struggled with Kubernetes! Running through Kubernetes the Hard Way was helpful for me understanding the basics of how K8s clusters work and how everything is wired together but still I struggled a little with the setup.

Overall - the things I was familiar with were (mostly) the things I did well on, and the new stuff I did less well on. That's okay - onwards and upwards!
