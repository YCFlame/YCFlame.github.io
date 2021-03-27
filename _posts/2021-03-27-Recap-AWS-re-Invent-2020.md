---
layout: post
title: Recap AWS re:Invent 2020
categories: ["AWS"]
---

![re:Invent](/images/AWS-reInvent.png)

I’m glad that people like my post [*How to Become a Google Certified Professional Cloud Architect*](https://medium.com/swlh/how-to-become-a-google-certified-professional-cloud-architect-87f2b5fe4a9b)*.* Google has sent me a hoodie and a mask for participating in their exam. However, [my employer Indeed selects AWS as its Preferred Cloud](https://www.businesswire.com/news/home/20200901005230/en/), so these gifts won’t stop me from pursuing certificates from the cloud leader. Amazon hosts [re:Invent](https://reinvent.awsevents.com/) annually to announce AWS updates. The just ended 2020 one would be the best chance to catch up with their latest progress.

This is the first time hosting the whole event online for safety. It’s both unlikely and unnecessary to watch all sessions of several thousand minutes in total. Here are my top 7 updates worth noting:

<!--more-->

**1.** [**S3 supports Strong Read-After-Write Consistency**](https://aws.amazon.com/about-aws/whats-new/2020/12/amazon-s3-now-delivers-strong-read-after-write-consistency-automatically-for-all-applications/)**.**

![Strong Consistency](/images/Strong-Consistency.png)

In other services, like [DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html), AWS already offered strong consistency with a price premium. But this time, Amazon S3 delivers strong read-after-write consistency automatically for all applications. You don’t need to write code to maintain “object”¹ consistency any more. Companies requiring state synchronization like Dropbox could [benefit a lot from this](https://www.youtube.com/watch?v=6x-XGJQwk2M). This is nothing revolutionary since Google’s counterpart [Cloud Storage already has this feature](https://cloud.google.com/storage/docs/consistency), but still, engineers could save their brains for other top priorities.

**2.** [**EC2 Mac instances**](https://aws.amazon.com/blogs/aws/new-use-mac-instances-to-build-test-macos-ios-ipados-tvos-and-watchos-apps/)**.**

![img](https://cdn-images-1.medium.com/max/1600/1*5c-Cw9rObjZQ5GEsgoWRSQ.png)Mac mini in the chassis

This is a great news for those who want to develop apps for Apple ecosystem on AWS. I have to say Amazon really surprises me with their implementation of Mac instances. They don’t build something like a bigger Mac Pro, but squeeze a Mac mini into their chassis. I think this is Amazon’s practical engineering style different from Google’s shining one.

**3. Fully managed container and serverless applications deployment service:** [**Proton**](https://aws.amazon.com/proton/)**.**

According to [Berkeley’s prediction](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2019/EECS-2019-3.pdf), serverless would be the future for the next 10 years’ cloud computing. With Proton, serverless and container-based applications could automate and manage infrastructure provisioning and code deployments with lower effort. It’s kind of like a “kubernetes” for more than just containers. Let’s hope it will not be so complex like kubernetes that [Google has to make an Autopilot feature to simplify its usage](https://www.theregister.com/2021/02/25/google_kubernetes_autopilot/).

**4.** [**Babelfish for Aurora database**](https://aws.amazon.com/rds/aurora/babelfish/) **to understand Microsoft SQL Server.**

Microsoft Azure, not Google Cloud Platform, is AWS’ main rival. They are very good at transferring their Windows/Office/SQL Server users into their cloud customers. AWS wants to defend their market share, but they don’t have Android or G Suit like Google, so now their potential customers could lift their programs and shift to AWS with no extra cost. They are about to make Babelfish open source so everyone could fix bugs and keep it updated with SQL Server.

**5.** [**SageMaker Feature Store**](https://aws.amazon.com/sagemaker/feature-store/)**.**

Machine learning is now literally everywhere. It’s like you can’t say your products use state of the art technology if there is no “learning” in it. AWS announced their “App Store” for reusing machine learning models via SageMaker. I don’t think you have to integrate this into every product, but it could eventually benefit your business if this ecosystem does give birth to some really amazing feature.

**6.** [**AWS Fault Injection Simulator**](https://aws.amazon.com/fis/)**.**

Netflix is famous for their [chaos engineering](https://netflixtechblog.com/the-netflix-simian-army-16e57fbab116). The only way to test your system resilience is killing part of your services and see what happens, because this is what reality is. You can now use an official tool instead of some framework from third parties, which is a safer way to keep your system safe.

**7. Fully managed** [**Grafana**](https://aws.amazon.com/grafana/)**,** [**Prometheus**](https://aws.amazon.com/prometheus/)**,** [**CloudShell**](https://aws.amazon.com/cloudshell/)**.**

“Cloud Native” tools to visualize your operational data, monitor your system and manage your resources. I’m kind of surprised that AWS didn’t have a cloud shell like GCP from the very beginning, maybe this is because they don’t own a web browser like Google.

------

I hope seven takeaways could fit in your memory since this magic number is said to be our information processing capacity at a time. Some of the products mentioned above are in preview state and not ready for business, and you could follow their links for more details. I will present my journey to AWS certificates in following articles soon.

------

[1] S3 is object storage for files, images, etc.

Cross-posted on [Medium](https://beyondchaos.medium.com/recap-aws-re-invent-2020-2f00e6f9250a).
