# Create Application in Instana

This article explains about how to create Application or Application Perspective in Instana.

<img src="../images/image-instana-waiops-integration.png">

## Pre-Requisite

- The `kubernetes based application` is deployed in an Openshift Container Platform or on Kubernetes Cluster.

- The `Instana agent` is deployed in the cluster.

- `Instana` is installed and already observing the cluster. 

## Objective

The Objective is to create Application Perspective for the kubernete based microservices application.

Here `iLender` application is deployed in `ilend-ns` namespace. 

Lets create Application Perspective  called `iLend`

## Steps

1. Click on `Application` in the left navigation menu.

<img src="images/4-application-00001.png">

2. Click on `Add` button in the bottom of the screen.

<img src="images/4-application-00002.png">

3. Click on `New Application Perspective` button.

<img src="images/4-application-00003.png">

4. Choose `Kubernetes or Container` menu 

5. Click on `Next` button.

<img src="images/4-application-00004.png">

6. Select `Kubernetes` option in the top.

7. Select `Kubernetes Namespace` option in the list box.

<img src="images/4-application-00005.png">

8. Select the namespace where your app is deployed. Here `ilend-ns` is the namespace. If your namespace is not listed here, try putting some load to the app.

9. Select  `All downstream` option.

10. Click on `Next` button.

<img src="images/4-application-00006.png">

11. Enter `Application Perspective Name`.

12. Select on `All Calls` Option.

13. Click on `Create` button.

<img src="images/4-application-00007.png">

14. Here is the application perspective screen for the app that you have created.

<img src="images/4-application-00008.png">

## Next Step

Application Perspective is created here. 

You can configure `Events`, `Alerts` and etc to complete Instana with Watson AIOps Integration.

Prev : [Create Instana Webhook in Watson AIOps Event Manager (NOI)](https://community.ibm.com/community/user/aiops/blogs/jeya-gandhi-rajan-m1/2021/09/08/ins-waiops-2-create-instana-webhook-in-waiops)

Next : [Create Custom Payload in Instana](https://community.ibm.com/community/user/aiops/blogs/jeya-gandhi-rajan-m1/2021/09/08/ins-waiops-4-create-custom-payload-in-instana)

Home : [Integrating Instana with Watson AIOps](https://community.ibm.com/community/user/aiops/blogs/jeya-gandhi-rajan-m1/2021/09/08/ins-waiops-1-integrating-instana-with-watson-aiops)


#### Released by :
- Jeya Gandhi Rajan M
- Vijaya Bhaskar R Siddareddi
- Vijay Sukthankar (Squad Leader)

Hybrid-Cloud Squad, GSI Labs

#ibmautomation

