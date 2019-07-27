# Idea for Codefundo++ 2019
This repository has idea for Microsoft Hackathon/Codefundo++ 2019 

## Basic Plan:
Elections, referenda, and polls are very important processes & tools for the smooth operation of a modern democracy. We are planning to build a django based web app that will be used for securing and enhancing the Election Process & Polling in India. Elections are under constant threat from criminal groups, that alter vote count and hijack polling booths. These groups also spread misinformation about the main candidates. This has a heavy influence on our Country's economy & Decision making process. To protect the virtue of democracy in our country, we would work on creating a web app that uses Microsoft AZURE's Blockchain technology and Django Framework (Python based). In our ideation, we will adress these issues: 

* **Problem:** Prior to the election process, hackers breach into the voter database and alter the records. So, during the elections voters can't ID themselves and cast a poll. Hackers then use this altered ID to cast false votes.

* **Problem:** Fake News and Information casts a big impact on the voters. It leads to formation of a false opinion among the voters. Hence, probability of a non-worthy candidate getting elected becomes high.

* **Problem:** Hacked Polling Machines. Hackers can target the software used by these machines, and then manipulate the vote count.


## Working Explained:

We will be using the following dictionary models :
1) ``` voter = {'voteRight': true, 'name' : 'name', 'address' : 'address', 'vote' : 'vote', previousBlockHash : '###', 'spouseHashValue' : '###'}  ```
2) ``` campaigner = {'campaignRight' : true, 'name': 'name', 'candidateName' : 'cN', 'party' : 'party', 'criminalData' : dictionary} ```
3) ``` newsInfo = {'topic' : 'topic-name', 'newsSnipps': dictionary} ```
4) ``` vote = {'voterId': 'ID', 'candidateName' : 'name', 'partyName' : 'party'} ```


* Our app will help voters to upload their ID info to the azure blockchain. All of the data will be asymmetrically encrypted via RSA algorithm & stored in multiple systems (Thanks to BlockChain tech.) & this will make it impossible to alter voter records.

* Our app will allow campaigners to register themselves, which would be connected to Azure Blockchain. Since blockchain is open and supports RTI (due to distributed version system), people can view the campaigning statements and verify whether it is false or not via the blockchain technology. Moreover, Blockchain verified campaigners can be given a special tag, which will allow voters to have a good opinion.

* After securing votes to the EVM, the votes will be constantly fed to blockchain (which is impossible to alter). EC authorities will be nodes of this blockchain. Whenever allegations are raised, they can crosscheck via blockchain.

## Dataset Used:
We will be using the **Open Government Data Platform India' dataset**. (Digital India initiative)

## Technologies & Frameworks:
* Django 
* Python
* CSS
* JavaScript
* Bootstrap
