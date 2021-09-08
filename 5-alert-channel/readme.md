# Create Alert Channels in Instana

This article explains about how to create Alert Channels in Instana.

<img src="../images/image-instana-waiops-integration.png">

## Pre-Requisite

- A Webhook should have been created in `IBM Watson AIOps Event Manager (NOI)` to receive event alerts from Instana. The Webhook generated URL should have been noted and be available to use here.

## Objective

The Objective is to create Alert Channel that points to the Webhook in `IBM Watson AIOps Event Manager (NOI)`.

## Steps to create Alert Channel

1. Choose the menu `Alert Channels` under the configuration section. 

2. Choose the `Add Alert Channels` button on the right. 

3. Choose the `IBM Watson AIOps Webhook` option from the list. 

<img src="images/2-alert-channel-00001.png">

4. Enter the values for the below fields as shown in the screenshot. 

- Name
- WebHook URL

Here `WebHook URL` referes to the URL noted while creating the webhook `IBM Watson AIOps Webhook`  in `IBM Watson AIOps Event Manager (NOI)`.

5. Click on `Create` button. 

<img src="images/2-alert-channel-00002.png">

7. Alert channel is created and available as below. 

<img src="images/2-alert-channel-00003.png">

## Next Step

Alert Channel is created here. You can create `Alert` to complete Instana with Watson AIOps Integration.

Prev : [Create Events in Instana](https://community.ibm.com/community/user/aiops/blogs/jeya-gandhi-rajan-m1/2021/09/08/ins-waiops-5-create-events-in-instana)

Next : [Create Alert in Instana](https://community.ibm.com/community/user/aiops/blogs/jeya-gandhi-rajan-m1/2021/09/08/ins-waiops-7-create-alert-in-instana)

Home : [Integrating Instana with Watson AIOps](https://community.ibm.com/community/user/aiops/blogs/jeya-gandhi-rajan-m1/2021/09/08/ins-waiops-1-integrating-instana-with-watson-aiops)



#### Released by :

Jeya Gandhi Rajan M
Vijaya Bhaskar R Siddareddi
Vijay Sukthankar (Squad Leader)

Hybrid-Cloud Squad
GSI Labs

#ibmautomation

