---
layout: page
title: Mining Crypto on Azure
subtitle: How to spend your Azure Free Credits
---

This guide will show you how to:
- Create an Azure account
- Create a Monero-Wallet
- Start mining
- What to expect

### Create an Azure Account

There are different options for getting an Azure account with free credits:

- If you don't already have one, you can sign up at [https://azure.microsoft.com/en-us/free/] to get 150$ of free credits.
You WILL need to provide credit card information, which is used to verify your identity (see [Azure FAQ](https://azure.microsoft.com/en-us/free/free-account-faq/)).

- If you are a **student**, you can register for free at [https://azure.microsoft.com/nl-nl/free/students/] and receive $100 to spend on Azure. You will **NOT** need a credit card to create your account.

- If you have an MSDN subscription (probably from work), you will be provided with 50$-150$ credits every month. This is a private subscription, and can not be monitored by others. So why not use it to mine some crypto?

### Create a Monero Wallet (XRM)

You need to create a wallet to store your hard-earned crypto in. I personally use Mymonero: [https://mymonero.com/], but you can use any XRM address for mining.

### Set-up 

- Create a resource group:

![ResourceGroups](assets/img/manage-resource-groups-add-group.png){:class="img-responsive"}

Here, you can chose the name & geographic location in which the group is created.

- Create the resources needed to mine XRM:

We will use the *Azure Batch* service to create cheap VMs that will run our mining script.
You can chose the number of VMs that you run:

F4's are the most efficient. The cost around 0.03$/hour (or 25$/month), and give a hashrate of 2 Kh/s.
F2's are half the price (12$/month) but give a lower hashrate of 0.8 Kh/s.
I would advice to run as many F4s as possible, and only use an extra F2 VM if you free credits allow it.
If you have an MSDN subscription it is best to keep make sure that you don't go over budget, as you than have to restart the VMs manually every month.



