---
title: What is Serverless Besides a Bad Name for Using Servers
published: false
description: When you hear the name "serverless" it's confusing because it is the opposite of what it means. This post will help you become confused less about serverless.
tags: serverless, web, jamstack, jamuary
---

Chances are you've heard the term serverless and are even using some form of ✨serverless magic✨ yourself. But software is confusing, and software terms even more so. When I started [learning about the JAMstack](https://www.netlify.com/blog/2019/10/30/whats-angular-in-the-jamstack-it-sounds-delicious/) it threw me for a loop. Talk about how the JAMstack doesn’t use servers but relies on [serverless](https://en.wikipedia.org/wiki/Serverless_computing) functions left me confused. **Spoiler alert**: this doesn't make sense because serverless computing _actually_ uses servers. In the hopes of clarifying one mystery I wanted to write a quick post on what serverless really means.

## What it is, tho

> [Serverless](https://en.wikipedia.org/wiki/Serverless_computing): is a cloud-computing execution model in which the cloud provider runs the server, and dynamically manages the allocation of machine resources. (via [Wiki](https://en.wikipedia.org/wiki/Serverless_computing))

Serverless is just a way of handling _how_ you are _using servers_. Instead of handling all the infrastructure and server operations yourself you're relying on a cloud provider. The cloud provider can help with [scaling](https://www.ibm.com/blogs/cloud-computing/2014/04/09/explain-vertical-horizontal-scaling-cloud/), [server provisioning](<https://en.wikipedia.org/wiki/Provisioning_(telecommunications)#Server_provisioning>), [capacity provisioning](https://en.wikipedia.org/wiki/Capacity_management), [patching](<https://en.wikipedia.org/wiki/Patch_(computing)>), and more (depending on the provider). This takes a lot of operational burden off of your team and can help solve potential problems like slow response due to bottleneck or expensive unused overhead. Like most [JAMstack best practices](https://jamstack.org/best-practices/), serverless provides a way to delegate more tasks so the dev team can spend more time innovating and creating features, not focusing on maintenance.

Why the term "serverless" was chosen is mind-boggling to me. Regardless, the use of such an arguably contentious name has generated a good amount of buzz. So many people have heard or know the term "serverless". I mean, I had _finally_ convinced my family that "the cloud" is just servers. Do you know how long it's going to take me to convince them that "server**less**" is servers!?! Thanks, internet.

## It's All About the Money

Although serverless is technically an execution model, you're mostly talking about a service. Adding more to the confusion pile, the pricing model of serverless is enough to throw you into a tizzy. Traditionally, the cost model for running your own server is usually [server capabilities] \* [uptime] or you pay upfront for what you think you'll use. In comparison, with serverless computing, cloud providers will charge based on the resources used. How much capacity is used or how many times something is executed can determine the cost for a service.

A nice part about this pricing model, and one of the main benefits of serverless, is that most providers won't charge you if your server is idle, isn't taking up a lot of memory or executing code a ton. This can cost a lot less because a server usually sits idle for a huge percentage of the time. Although it's great to be able to hand your server reins over to a cloud provider you'll want to understand how often your code is executing and how your app is using memory to avoid a financial [foot gun](https://en.wiktionary.org/wiki/footgun).

## Key Takeaways

- serverless uses servers
- cloud providers handle the server operations
- pricing is usually quite confusing
- naming things is hard

I hope this helps shed some light onto one of the key elements of the JAMstack. The awesome [Jason Lengstorf](https://twitter.com/jlengstorf) has a whole series coming out this #JAMuary to help you wrap your mind around serverless functions. Keep your ear to the ground for that. In the meantime here are some other resources to peruse. Happy coding!👩🏻‍💻

Resources for the Road:

- [Netlify Functions](https://www.netlify.com/products/functions/)
- [Going Serverless with VueJS talk by Divya Sasidharan](https://www.youtube.com/watch?v=Mu9zKpGhX1Y)
- [Super simple start to serverless by Kent C. Dodds](https://kentcdodds.com/blog/super-simple-start-to-serverless)

p.s. I use a lot of handy Wiki links here, if you feel so inclined to thank them for this you can donate [here](https://wikimediafoundation.org/support/).
