## Building and Leading a Privacy-First Startup – Interview with Daniel Huynh

We, at the AI Time Journal, thank Daniel Huynh from Mithril Security for taking part in the Data Science Interview Series and sharing several insights on his journey to building and leading a privacy-first startup.

## Academic Background
**🎙️ Bala: Could you tell us about your academic background?**

**Daniel**: I am a recent graduate from Ecole Polytechnique and HEC Paris. So, I have an Engineering and a Business Analytics background. I chose to focus on Applied Math and Data Science during my study at Ecole Polytechnique.

## Getting Started with Privacy-Preserving Technologies
**🎙️ Bala: When did you realize that you were interested in Privacy and Privacy-Preserving Technologies?**

**Daniel**: I first got interested in Privacy-Preserving Technologies in 2019 when I came across a workshop organized by OpenMined in Paris. I really dug into this subject in 2020, during my internship at Microsoft, where I worked under the supervision of the CTO of Microsoft, France. There, I spent time studying how Homomorphic Encryption, Secure Multi-Party Computation and Confidential Computing work.

## Building a Privacy Tech Startup
**🎙️ Bala: What inspired you to build a startup in the privacy tech space?**

**Daniel**: It all started during my internship at Microsoft. I heard that a major health company had a leak due to a third party partner who got compromised. I thought it was a shame, especially in Covid times, but it’s the kind of thing that could happen when you collaborate with someone and there is no point in shaming this partner.

> I thought, “Wouldn’t it be great if anytime you need to collaborate with a third party, because they provide you a service or service you don’t want to have in-house – and they do it without seeing your data directly but still do it?”

Then I linked this idea with what I was doing at Microsoft, and understood that the recent technological advances have made this possible, but there are still not many products available out there to democratize these technologies. 

Thus, I  decided to start Mithril Security to turn these state-of-the-art techniques into a product that could be used by many organizations to collaborate, share, and analyze data, without risking the privacy of their data.

**🎙️ Bala: As the CEO of Mithril Security, could you tell us about the exciting services that Mithril is currently working on?**

**Daniel**:  Our goal is to help AI providers deploy privacy-friendly models to apply AI models to their users’ data without having direct access to the data, thanks to end-to-end encryption!

To achieve this, at Mithril Security we are developing a secure AI inference using Confidential Computing. Our inference server simply takes as input your exported AI model, usually as an ONNX file, and serves it securely to the end users using our client SDK.

> Our goal is to make our services as transparent and easy as possible, both for the AI engineers and end-users, without compromising on security and speed.

That is why we have chosen to ingest ONNX files, as it is already commonly done, and provide a Python SDK (other languages will be available in the future), to make it easy to securely share data for consumption by an AI model.

We will soon release a series of articles showing how it works in practice, from the training and export of the model, to the consumption by the end user. We have a few scenarios that we can already cover: 

- Email classification as a service to detect if an email is a spam/phishing attempt, without having access to the content of the email
- Using Transformers
- Confidential Semantic Search with word2vec
- Private Biometric Authentication with a Siamese network

## Challenges in Deploying Privacy-Preserving ML services
**🎙️ Bala: What’s your opinion on the deployment of Privacy-Preserving ML services? What are the major bottlenecks that come in the way of deploying such services at scale?**

**Daniel**: As of today, the deployment of Privacy-Preserving ML services seems close yet far. Most of the results we see today show slowdowns that are too important for a real deployment. There is also the problem of making it easy to use for AI engineers.

Because the experts building the privacy-preserving tools are not always aware of the current toolkits and best practices in the Data Science community – there might be a gap between what is offered today, and what users want.

**🎙️ Bala: As a leader in the Privacy-Preserving tech industry, could you summarize the greatest challenges and milestones at Mithril Security?**

**Daniel**: Following my previous point, we at Mithril Security aim to provide a product that provides the best balance between speed, security and ease of use. Having a solution that performs well on these three points at the same time is highly non trivial, and we seem to be getting there as our secure inference server can run models with a x2 slowdown, for instance a MobileNet, while securing data in use – all this  with a simple interface for the AI engineer and the end user.

While we focused on making fast inference for a single server, we still have to work on the scaling and load balancing, certification of our product and user experience. 

I believe communication and building an awesome community for our product are also key factors to make our product advance and reach mass adoption by the Data Science community.

**🎙️ Bala: Could you recommend good learning resources for Privacy-Preserving ML?**

**Daniel**: OpenMined is the first resource that comes to my mind, with its privacy course – The Private AI Series. There are also articles you can find on blogs, such as OpenMined and on Medium. You can find my series on CKKS, an Homomorphic Encryption scheme, as well as the one we have started on Confidential Computing.

**🎙️ Bala: Could you summarize in two lines the potential use cases of Privacy-Preserving ML?**

**Daniel**: I think the use cases of Privacy-Preserving ML are limitless and any classic ML use case can benefit from Privacy-Enhancing Technologies (PETs). But the most natural use cases would be AI-assisted decision making, voice assistants, and corporate documents analysis.
