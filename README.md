# aws-security-policies

In the world of cloud computing, I’ve been rolling up my sleeves as an IAM engineer, diving deep into ways to tighten up security and streamline how we manage resources in AWS. My goal? To make everything more secure and run smoother.

Firstly, I realized we needed a better way to control who could send messages to our SNS topics. It was all about keeping our data exchanges clean and secure, so I set up a policy that ensures only the right people and services can publish messages. This was a big step in keeping our communications tight.

Then, I tackled another big challenge: keeping our core AWS resources safe from any unauthorized changes. I whipped up a Service Control Policy that put up some serious guardrails, making sure only a few trusted hands could make changes to our critical setups.

Cost management was up next. We definitely didn’t want to overspend on resources we didn’t need, especially in our testing environments. So, I put together a policy that keeps our EC2 instances small and budget-friendly when we’re just testing the waters, making sure we’re not using more than we need.

Lastly, there was the tricky issue of the confused deputy problem—it’s a bit like if someone tricked a sheriff into locking up the wrong person. I had to ensure that our AWS services couldn’t be manipulated by someone from outside to mess with our resources. So, I created a policy that really narrows down who can tell our S3 service to do things like sending notifications to our SNS topics.

All in all, putting these policies together taught me a ton about the ins and outs of AWS’s tools and how carefully managing access can make a huge difference in security and efficiency.

Reflecting on all this work, I feel pretty good about the safer, more cost-effective environment we’ve crafted. Plus, I’ve shared all this in a GitHub repo, hoping it might help others facing similar challenges. It’s all about making the cloud a better place for everyone!

My source of inspiration is an AWS workshop : https://catalog.us-east-1.prod.workshops.aws/workshops/d1531d0a-79fd-45af-b198-d81e349ee660/en-US/20-install-the-assessment-tool
