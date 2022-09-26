<h1>Make your environment Zero Trust compliant</h1>

    *This document describes our team social contract for this project*

<ul>
<li>Brandon is working on Encryption/Exchange</li>
<li>Christian is working on Firewall/Port Setup</li>
<li>Shaq is working on Initial Login</li> 
<li>Mark is working on Recovery</li>
<li>Daniel is working on Authentication/Security Authority</li>
<li>Record issues that are non-blocking and discuss right after lunch at re-group meeting</li>
<li>Bring up any blocking issues after 15 minutes of spinning your wheels on Slack</li>
<li>At 2:30pm have re-group meeting where you check-in with blockers, status updates and plan</li>
</ul>

Team expectations
    <ul>
        <li>Each of us reserves the rights to our nights and weekends, and shall discuss any necessary usage on private time for group effort</li>
        <li>If you have a blocking issue, slack before interrupting another’s train of thought</li>
        <li>Share the mic</li>
        <li>Be willing to discuss progress, even if minute. Progress is progress</li>
        <li>Always message the group when you change what you are working on - it is ALWAYS better to over communicate in a remote setting</li>
        <li>Use the team slack with your team members to keep your fellow and instructors well-informed</li>
    </ul>
If the group is divided on a certain decision we will take the following steps
    <ol>
        <li>Take 10-15 minute break</li>
        <li>List out the pros / cons</li>
        <li>Vote on it! If the vote is split, escalate to a 3rd party</li>
        <li>If you are frustrated, Take a walk or get some water</li>
        <li>Bring in a 3rd party (e.g. senior tech lead) to mediate if you feel too frustrated</li>
    </ol>

<h1>WHY ZERO TRUST?</h1>

The Traditional Networking security approach was built to protect the data center with four high walls. Logically, there is only one front door, which is used as the only point for network traffic to come in and go out. The Security guard at the front door will filter the network traffic coming in and going out. In this approach the Security guard represents the network middleware appliances securing the data center. Everything inside the walls or network is trusted traffic, inside a trusted zone, and everything outside the wall is untrusted. Common network middleware appliances are Firewalls at OSI layer level 4, Web Application Firewalls (WAF) at level 7, Intrusion detection systems, Intrusion prevention systems, & Security information and event management systems. VLAN may also be used to further protect the network by using segmentation. Segmentation will split the network into sub networks and restrict communication between different sub networks. This is the Traditional Perimeter Security Model. Most organizations are a using a mix of cloud services, servers, devices, and organizational units.Traditional Perimeter Security is very difficult to manage in a world of microservices.


We must eliminate the notion of a trusted network (intranet) and an untrusted network (external networks). In Zero Trust, all network traffic is untrusted.
