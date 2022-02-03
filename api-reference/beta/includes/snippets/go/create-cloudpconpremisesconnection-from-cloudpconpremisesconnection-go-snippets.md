---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fcc3dc4cf9462816803529e72bfe14217e18c02
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351490"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcOnPremisesConnection()
displayName := "test-canary-02"
requestBody.SetDisplayName(&displayName)
type := "hybridAzureADJoin"
requestBody.SetType(&type)
subscriptionId := "0ac520ee-14c0-480f-b6c9-0a90c585ffff"
requestBody.SetSubscriptionId(&subscriptionId)
subscriptionName := "CPC customer 001 test subscription"
requestBody.SetSubscriptionName(&subscriptionName)
adDomainName := "contoso001.com"
requestBody.SetAdDomainName(&adDomainName)
adDomainUsername := "dcadmin"
requestBody.SetAdDomainUsername(&adDomainUsername)
organizationalUnit := "OU=Domain Controllers, DC=contoso001, DC=com"
requestBody.SetOrganizationalUnit(&organizationalUnit)
resourceGroupId := "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG"
requestBody.SetResourceGroupId(&resourceGroupId)
virtualNetworkId := "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET"
requestBody.SetVirtualNetworkId(&virtualNetworkId)
subnetId := "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet"
requestBody.SetSubnetId(&subnetId)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
}
options := &msgraphsdk.OnPremisesConnectionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnections().Post(options)


```