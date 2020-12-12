---
layout: post
title: How To Become A Google Certified Professional Cloud Architect
categories: [GCP]
---

![GCP Professional Cloud Architect](/images/badge.png)

After about two months’ preparation, I got my Professional Cloud Architect certificate this week. This experience gives me a lot on [Google Cloud Platform](https://cloud.google.com/)(a.k.a. GCP) and architecture design principles. The exam is not difficult at all for a veteran engineer, and I haven’t tried GCP before in my life. I’ll explain how to pass it quickly, and how you can get the most of it rather than just a certificate.
<!--more-->

## Why GCP Cloud Architect

![2020 Q3 Cloud Market Shares](/images/Q3-Cloud-Shares.jpg)

According to [Canalys’ report](https://www.canalys.com/newsroom/worldwide-cloud-market-q320), Google only possesses 7% of the whole cloud market in Q3 this year, comparing to Microsoft’s 19% and Amazon’s 32%. Amazon’s AWS stepped into this arena first, and Microsoft Azure expands its share from Enterprise customers who using Windows and Office. It must be very difficult for Google to catch up, so why choose a GCP certificate now?

![Cloud Certifiate Ranking](/images/certificate-ranking.png)

Global Knowledge said in [15 Top-Paying IT Certifications for 2020](https://www.globalknowledge.com/us-en/resources/resource-library/articles/top-paying-certifications/) that GCP Cloud Architects earn an average of $175,761 in the U.S., about $26,000 more than AWS Certified Solutions Architect per year. A possible reason would be the supply-demand relationship: Engineers with Cloud Architect certificate aren’t enough in the market. You may choose AWS if you want to fit in more positions, but a GCP Cloud Architect certificate may take your career to the next level.

I choose GCP for three more reasons. First, it’s Google who published three papers(GFS, MapReduce, Bigtable) opening our minds to large-scale distributed systems. Almost every engineer who cares about scalability would be familiar with these concepts. This makes you feel natural about products on GCP rather than AWS. And Google is always standing on the frontier of technology, you could anticipate that the cutting edge research would soon be integrated into their platform, keeping yourself competent in the industry.

Second, you definitely want to take a remote exam rather than going to a test center spending hours with other candidates, while the coronavirus is still not under control in most of the world. However, Amazon didn’t allow candidates in China, Japan, Slovenia, and South Korea to take online proctoring exams when I decided to get a cloud certificate months ago. In October, they finally [increased availability for these people](https://aws.amazon.com/about-aws/whats-new/2020/09/increased-availability-for-aws-certification-exam-online-proctoring/). For candidates now, you can pay $300 to take a 3-hour AWS online test or $200 for a 2-hour GCP one. But be careful, an AWS certificate is valid for 3 years while a GCP one for 2 years. You can take a renewal exam for half a price when they are expired.

Last but not least, GCP Cloud Architect is more on high-level principles while their Cloud Engineer or Cloud Developer is more on platform details. It’s both easier and more meaningful if you can focus on the big picture and skip the command line parameters at first. After all, you can always refer to the manual, why bothering to pay for it.

## Which resources are handy

There are millions of search results throwing tons of references to you. However, I think you don’t need to become a library to get a certificate. When you register an account on [Google Cloud Certification](https://cloud.google.com/certification), they would provide you some materials to prepare. I found the most valuable resource is the ebook named **Official Google Cloud Certified Professional Cloud Architect Study Guide**. You can purchase it for $19.99 with their coupon. This book covers every aspect of the exam, arming you with exercises after each chapter and an assessment test of 25 sample questions. The content is more concentrated than Google’s own documents so you could get familiar with the exam quickly. Also, you can register a new account on Coursera to access 6 courses for free in the first month. These courses would be more fun than plain text in the ebook, and you can get your hands dirty on Google Cloud Platform to solve the quizzes. Teachers would teach you how to design a system considering the requirements besides details of the platform, which would benefit your career in general.

After finishing the reading and lessons, you will find [official sample questions](https://cloud.google.com/certification/sample-questions/cloud-architect) and [practice tests on whizlab](https://www.whizlabs.com/learn/course/gcc-pca-pt/) really helpful before the exam. Use these tests to get familiar with question forms and UI. There are only two types of questions: multiple choice and multiple select. You even get hints of how many answers to be chosen. In my experience, whizlab’s practice questions are more difficult than the real ones in my exam. You can use them to identify your weaknesses and don’t get entangled in specific details or the score you get. I got no more than 80% accuracy in all these tests, which is said to be the pass line, yet still got my certificate.

## Which parts are tricky

The most important part is to design a solution meeting both business and technical requirements. This normally involves three sample case studies offered by Google: [Mountkirk Games](https://cloud.google.com/certification/guides/cloud-architect/casestudy-mountkirkgames-rev2), [Dress4Win](https://cloud.google.com/certification/guides/cloud-architect/casestudy-dress4win-rev2), [TerramEarth](https://cloud.google.com/certification/guides/cloud-architect/casestudy-terramearth-rev2). They are also typical architecture models in the current industry: online game craving for scaling both up and down, e-commerce website with high availability and transactional deals, IoT network aiming for high volume stream analysis. There are different ways to look into their problems, which could bring solutions from different domains.

To be specific, you need to consider GCP computing instances, storage services, big data analysis tools, load balancers, CDN, network infrastructures, security measures, legal compliance, data migration plans, etc. For experienced engineers, just get familiar with [Google Cloud Products](https://cloud.google.com/products) and choose from them based on the situation. If you haven’t made trade-offs that much, it will be very helpful to read the ebook and answer questions to figure out why they are like that.

Among all of these, **network, security, legal compliance** would be relatively unfamiliar to developers, because we are not even aware of them in our daily coding, testing, deploying and monitoring process. Site reliability engineers, security engineers and lawyers handle them for us, so this may be a good chance for you to know what an Architect needs.

## What's next

Now you are a Professional Cloud Architect, what does it mean? It could mean almost nothing because you don’t even need engineering experience to nail the exam, many salespeople passed this. It’s like you can’t say you are a native speaker after passing some language exam. However, you could become a real architect if you keep using what you learned in real-life engineering. Assessing business and technical requirements, design your architecture for scalability and reliability, choosing or even crafting services to fulfill them, monitoring your system for debugging and performance tuning, working with other colleagues to prevent security and legal problems, are what an architect means, not a digital certificate.

Large scale distributed systems are the only solution for worldwide companies. You need to dive into the Google Cloud Products figuring out why they could face the challenge. CAP Theory, relational databases, NoSQL, stream computing, consistency, etc. [Official documents](https://cloud.google.com/docs) would be your best friends now. Why spanner could be a worldwide relational database and Cloud SQL can’t? Why BigTable could handle intense concurrent writing? Why Cloud Function could be so lightweight making serverless real? You will get the most of this certificate if you keep hungry for these non-trivial problems and answer them. Even better if you can solve problems that Google can’t.

------

Cross-posted on [Medium](https://beyondchaos.medium.com/how-to-become-a-google-certified-professional-cloud-architect-87f2b5fe4a9b).