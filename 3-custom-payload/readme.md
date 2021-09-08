# Create Custom Payload in Instana

This article explains about how to create Custom Payload in Instana.

<img src="../images/image-instana-waiops-integration.png">

## Objective

The Objective is to create Custom Payload. By doing this whenever there is an alert send from the Instana to any alert Channels, the data could contain what is mentioned in the Custom Payload as well.

This helps the Instana to send additional info along with the alert data to the alert channels.

The custom payload would look like this. Look at the section `customPayloads`

```
{
    "details": {
    "containerNames": [],
    "customPayloads": {
      "custom:NodeAlias": [
        "ilender-creditscore-66d5886bd9-vl2xk"
      ]
    }
  },
  "deduplicationKey": "someId",
  
  "sender": {
    "name": "Instana",
    "displayName": "Instana Server",
    "sourceId": "someId",
    "type": "Instana"
  },
  "resource": {
    "sourceId": "someId",
    "type": "JVM",
    "displayName": "test",
    "hostname": "test.fqdn",
    "name": "test"
  },  
  "severity": "Warning",
  "summary": "Garbage Collection Activity High (11%)",

  "type": {
    "eventType": "JVM"
  }
}
```

## Steps

1. Choose the menu `Custom Payload` under the configuration section. 

2. Click on `Add Row` button. 

<img src="images/image-1.png">

3. Enter the `Node Alias` in the field `Custom`. 

4. Choose  `Dynamic` in the field `value type`. 

5. Choose  `Kubernetes Pod Name` in the field `value`. 

6. Click on `Save` button. 

<img src="images/image-2.png">

Now all the alerts send from this Instana would have Kubernetes Pod Name inside the alert data.

```
    "customPayloads": {
      "custom:NodeAlias": [
        "ilender-creditscore-66d5886bd9-vl2xk"
      ]
    }
```    


## Next Step

Custom Payload is created here. 

You can configure `Events`, `Alerts` and etc to complete Instana with Watson AIOps Integration.

Prev : [Create Application in Instana](https://community.ibm.com/community/user/aiops/blogs/jeya-gandhi-rajan-m1/2021/09/08/ins-waiops-3-create-application-in-instana)

Next : [Create Events in Instana](https://community.ibm.com/community/user/aiops/blogs/jeya-gandhi-rajan-m1/2021/09/08/ins-waiops-5-create-events-in-instana)

Home : [Integrating Instana with Watson AIOps](https://community.ibm.com/community/user/aiops/blogs/jeya-gandhi-rajan-m1/2021/09/08/ins-waiops-1-integrating-instana-with-watson-aiops)


#### Released by :

Jeya Gandhi Rajan M
Vijaya Bhaskar R Siddareddi
Vijay Sukthankar (Squad Leader)

Hybrid-Cloud Squad
GSI Labs

#ibmautomation

