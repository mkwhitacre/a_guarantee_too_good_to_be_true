# A Guarantee Too Good To Be True

This repository holds the slides from a presentation given at [Cerner DevCon](https://engineering.cerner.com/) 2020.

# Abstract
The opportunity for failure exists everywhere in our architecture.  The failures can even exist when you are running on a single machine.  As products look to adopt a more distributed architecture for processing, queueing, and microservices, the opportunity for failure increases.  Despite research and theorems that prove we cannot achieve perfection, the marketing for various distributed technologies talk about how they solve the failure problem.  So can we really trust a processing engine that says it supports exactly-once processing?  Can we trust a data storage system that says it supports ACID?  Are you excited about this new technology because it promises to solve all of your problems?

The answer is “it depends”.  Starting with a common foundation of research, we can start to evaluate if a technology really lives up to its promises.  Specifically digging into the internals of industry standard technologies for processing and data storage, we can see how they can even attempt to solve the failure problem but also practically achieve their guarantees.  The answer will reveal that their guarantees are often based on specific interpretations of terms or only under certain conditions and not universal.

Understanding that nothing is perfect and building up the skill sets to do proper technology evaluation will help you see that nothing is really magic.  It also will help us to avoid assumptions that might lead to difficult bugs or issues when the guarantees do not live up to the promise.  This talk will hopefully instill enough skepticism and curiosity to dig past the promises to see what you are really getting.  Overall we will be able to understand that if something seems too good to be true it likely is.
