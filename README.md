Zero Trust Linux Setup 101
Basic Kali setup to make your environment framework Zero Trust compliant
*This document describes our team social contract for this project*
Daily process

Work on tasks chosen/assigned in groups or solo as declared
Brandon is working on Encryption/Exchange
Christian is working on Firewall/Port Setup
Shaq is working on Initial Login 
Mark is working on Recovery
Daniel is working on Authentication/Security Authority
Record issues that are non-blocking and discuss right after lunch at re-group meeting
Bring up any blocking issues after 15 minutes of spinning your wheels on Slack
At 2:30pm have re-group meeting where you check-in with blockers, status updates and plan

Team expectations
Each of us reserves the rights to our nights and weekends, and shall discuss any necessary usage on private time for group effort
If you have a blocking issue, slack before interrupting another’s train of thought
Share the mic
Be willing to discuss progress, even if minute. Progress is progress
Always message the group when you change what you are working on - it is ALWAYS better to over communicate in a remote setting
Use the team slack with your team members to keep your fellow and instructors well-informed
Issues
If the group is divided on a certain decision we will take the following steps:
Take 10-15 minute break
List out the pros / cons
Vote on it
If the vote is split, escalate to a fellow or instructor
If you are frustrated
Take a walk or get some water
Talk constructively about actionable items (e.g. raise your hand instead of interrupting, let me learn and struggle until I ask you for help, etc.)
Bring in a 3rd party (e.g. fellow, instructor) to mediate if you feel too frustrated



WHY ZERO TRUST?

The Traditional Networking security approach was built to protect the data center with four high walls. Logically, there is only one front door, which is used as the only point for network traffic to come in and go out. The Security guard at the front door will filter the network traffic coming in and going out. In this approach the Security guard represents the network middleware appliances securing the data center. Everything inside the walls or network is trusted traffic, inside a trusted zone, and everything outside the wall is untrusted. Common network middleware appliances are Firewalls at OSI layer level 4, Web Application Firewalls (WAF) at level 7, Intrusion detection systems, Intrusion prevention systems, & Security information and event management systems. VLAN may also be used to further protect the network by using segmentation. Segmentation will split the network into sub networks and restrict communication between different sub networks. This is the Traditional Perimeter Security Model. Most organizations are a using a mix of cloud services, servers, devices, and organizational units.Traditional Perimeter Security is very difficult to manage in a world of microservices.

BeyondCorp is a security model that allows Google employees to work more securely from any location without the need for a traditional VPN.

The BeyondCorp Zero Trust Model Implementation by Google is logically the same as a Zero Trust Architecture.

We must eliminate the notion of a trusted network (intranet) and an untrusted network (external networks). In Zero Trust, all network traffic is untrusted.