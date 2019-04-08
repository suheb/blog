---
layout: post
title: Linux Chix Delhi Meetup
date: 2017-10-21 19:22
summary: My experience as a speaker at Linux Chix Delhi meetup
categories: meetup speaker
---

I procrastinated writing this blog for over a month now. To be honest, I'm not much of a writer but I love to read. I read up pretty much anything I can get my hands on. Recently, I also started reading the blog posts from my idols, my friends, and my nemesis. Reading about people's experiences made me want to share mine. Perhaps I could write something too that people will love to read.

I recently attended the LinuxChix meetup in Delhi where I was invited as a speaker to talk about "How SSH works?". I reached the venue 15 minutes before my talk was scheduled. The one thing that struck me the most the moment I entered the room was the dearth of _Chix_. Being a LinuxChix (a women-oriented Linux community.) meetup, I expected to see a lot of girls. But apart from the two coordinators, there were only two other girls and one of them was the speaker. Sadly, this is the state of women in technology.

I started my talk by giving a brief introduction of SSH. I shared a little story about [how ssh got the now famous port 22](https://www.ssh.com/ssh/port#sec-The-story-of-getting-SSH-port-22) which the attendees loved. After that, I described the various encryption and hashing algorithm used in SSH. There is a common misconception that SSH uses _asymmetric key encryption_. This notion is so widespread because the most commonly used method to authenticate the client does use asymmetric key encryption. This is the part where you get a prompt _like this_ in your terminal window.

{% highlight terminal %}
$ ssh -T git@github.com
/# Attempts to ssh to GitHub
The authenticity of host 'github.com (IP ADDRESS)' can't be established.
RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
Are you sure you want to continue connecting (yes/no)?
{% endhighlight %}

But that's not the case. SSH uses _symmetric key encryption_ to set up a secure channel for server and client to communicate.
When you get the above prompt, the secure channel has already been established using symmetric key encryption behind the hood.

I continued on to describe the whole process of establishing a secure channel in a lot more detail. I described where and how this process differs in SSHv1 vs SSHv2. I concluded my talk with some applications of ssh and where it's most commonly used.

After my talk, there were two other talks scheduled that day. Both of them by my fellow colleagues and good friends at Zomato.

First, [Anu Mittal](https://github.com/Anumittal) talked about [the history of Linux and her experience](http://anu-mittal.blogspot.in/2017/09/linuxchix-meet-up-experience.html) working on it. It was a really inspiring talk for all the young attendees at the meetup who're just getting started with Linux, especially for the girls.
After that, [Garvit Khatri](https://github.com/garvitdelhi), who was late as always, talked about the [Filesystems in Linux](https://garvit.in/2017/09/18/linuxchix-meetup.html). The talk was really informative as I realized how much I don't know about Linux filesystems. My heartiest congratulations to both the speakers on such wonderful talks.

I would also like to congratulate the organizers, [Shivani Bhardwaj](https://github.com/shivan1b) and [Priyal Trivedi](https://github.com/Priyal-Trivedi), for their continued efforts to keep this amazing community going.

That's it from my first blog. Hope you enjoyed it.
Until next time!
