# Idea for Codefundo++ 2019
Elections, referenda, and polls are very important processes & tools for the smooth operation of a modern democracy. Build a Proof-of-Concept to demonstrate how you can make these processes more secure, reliable, and transparent using Blockchain.

## Basic Plan:
Elections and polls being a crucial procedure for upholding the basic virtue of democracy should be completely a representative of public opinion. But in almost all modern-day large democracies like in India, malpractices are being conducted to breach smooth conduct of elections by major political groups, individual leaders, militant groups, big media houses and others who benefit from such practises. These malpractices include spreading fake information about candidates through various media, manipulating voter's information, altering vote count, hijacking polling booths, increasing role of moneypower in election campaigning, using big data Analytics firm to use data for benefit in elections. 
To protect the virtue of democracy in our country, we would work on creating a web app that uses Microsoft AZURE's Blockchain technology and Django Framework (Python based). In our ideation, we will address the following issues.

## Problems:
1) Prior to the election process, **hackers breach into the voter database** and alter the records. So, during the elections voters can't verify themselves and cast a vote. Hackers then use this altered ID to cast false votes. 

2) **Fake News and Information** casts a big impact on the voters. It leads to formation of a false opinion among the voters. Hence, probability of a non-worthy candidate getting elected becomes high. Also candidates with money power pay money to **big data Analytics** firm to gather voter's information like their interests, contact details, credit card transaction history, stance on particular issue etc.Then they conduct their campaign according to the information gathered to edge over other candidates in the elections.

3) **Hacked Polling Machines**. Hackers can target the software used by EVM's, and then manipulate the vote count. Also, sometimes voters are made to forcefully vote for a political party or individual leader.  

## Working Explained:
First of all, taking example of elections in India, we will be using Aadhaar Card along with Voter ID for unique identification, registration, and manipulation of voters' information. Role of Election Commission in mentioned in each point. For voters information, campaigner details,news and messages, vote count we intend to make five chains namely voter_info, campaigner and news_Info and campaign_message (for each constituency in General ELections) and vote. 
We will be using the following data structure to create data objects in these blockchains respectively:
1) ``` voter_info = {'name' : 'voter_name', 'address' : 'voter_address', 'election_voted' : list,'aadhaar':Aadhaar Number}  ```
2) ``` campaigner = {'campaignRight' : true/false, 'name': 'campaigner_name', 'candidateName' : 'cN', 'party' : 'party'/none, 'is_police_verified' : true/false,'campaigner_bio':'(information about campaigner)'} ```
3) ``` news_Info = {'topic' : 'topic-name', 'newsSnipps': dictionary} ```
4)``` campaign_message = {'topic' : 'topic-name','message':dictionary,'campaigner':'campaigner_name','candidate':'candidate_name'} ```
5) ``` vote = {'voterId': 'ID', 'candidateName' : 'name', 'vote' : integer(indicating candidate voted),'for_election':'election_name'} ```


* Our app will help voters to upload their info to the azure voter_info blockchain. All memebers of a special team for unique identification, registration, and manipulation of voters' information in EC will be nodes of this blockchain. All of the data (eg. voter data structure mentioned above) will be asymmetrically encrypted via RSA algorithm when it is transfered & stored in multiple systems (Thanks to BlockChain tech.). This will make it impossible for hackers to alter voter records. Any genuine attempt to change information is proposed to be done through biometric verification which uses Aadhaar information of candidates. 

* Our app will allow campaigners to register themselves, which would be connected to Azure campaigner Blockchain specifically for that constituency. This blockchain will be open (due to distributed version system) to all registered voters in that constituency, enabling people to know the campaigner's background. Blockchain verified campaigners can be given a special tag, which will allow voters to have a good opinion.
As explained earlier the use of of big data analytics in the election,to deter it, we intend to stop people from getting personalised campaign messages by allowing campaigners to upload generalised messages on the forum and  azure campaign_message blockchain. This blockchain will also be open to all registered voters in that constituency. This will reduce the role of big data analytics in modern elections and hence role of moneypower. Moreover, this will help to have a proof of promises made by candidates so that they can be reliably questionned later. Obviously,EC need to encourage people to view mesaages on this media instead of any other media.
To prevent Fake News and Information to change public opinion we intend to have azure news_info blockchain in each constituency to keep track of all political news circulated in the campaign period in that constituency. All the EC officials responsible for that constituency will be nodes of the blockchain and they will verify the news as fake or not. It will be surely a huge task and work should be done using proof-of-stake and modern softwares capable of classifying news as fake. 
* During polling votes to the EVM, the votes will be constantly fed to vote blockchain (which is impossible to alter). All EC authorities will be nodes of this blockchain. Whenever allegations are raised, they can crosscheck via blockchain the vote count. In case of forceful polling for an individual, there will be provisions for a voter to track and change vote later via app signing in through biometric recognition (through Aadhaar card) during polling period. 

## Dataset Used:
We will be using the **Open Government Data Platform India' dataset**. (Digital India initiative)

## Technologies & Frameworks:
* Microsoft Azure Blockchain
* Microsoft Azure Cloud
* Django 
* Python
* CSS
* JavaScript
* Bootstrap
