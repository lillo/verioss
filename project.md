
## The VeriOSS Project 

Here we provide a brief description of the main goals of VeriOSS.
For a more detailed presentation, read our main [paper](https://iris.imtlucca.it/retrieve/handle/20.500.11771/15589/13805/main.pdf).

### What are bug bounty programs? 

Bug bounty programs are essential to attract skilled software analysts for the detection, disclosure and correction of software errors.
In such a program, a *bounty issuer* (BI), typically the developer of a piece of software, offers a reward to any security expert, aka *bounty hunter* (BH), who discovers a bug her software. 
The offered reward usually depends on the typology and criticality of the bug. 

Currently, many platforms exist that foster these programs, see for example [Hackerone](https://www.hackerone.com/) and [Intigriti](https://www.intigriti.com/).

### What are the main challenges of bug bounty platforms?

The current market of bounty is inefficient, mainly due to lack of commitment with respect to the eligibility of bugs.
Indeed, a BH is usually expected to disclose all details of a bug to the BI who then decides on the severity of the bug and therefore how much to
pay. 
Clearly, the BI has strong incentives to "downgrade" the bug or declare it not eligible for the bounty. 
This inefficiency pushes BHs to look for other opportunities, such as gray and black markets.

### What is the goal VeriOSS?

Our goal is to create a fair bounty market, so as to
foster more bug hunting and, consequently, decrease the appeal of grey and black markets.

In particular, VeriOSS has two goals: 
1. support an honest bounty hunter BH in collecting a reward under the assumption of an untrusted bounty issuer BI; 
2. protect BI against untrusted BHs claiming an undeserved reward.

VeriOSS achieves these two goals by 
1. requiring BI to provide a precise description of the eligible bugs;  
2. driving the BH in disclosing the bug and claiming for the reward.

The code of VeriOSS is a bug disclosure protocol that is arbitrated by a smart contract.
At the end of the protocol, BI will obtain the full disclosure of the bug and BH will receive the expected reward.
