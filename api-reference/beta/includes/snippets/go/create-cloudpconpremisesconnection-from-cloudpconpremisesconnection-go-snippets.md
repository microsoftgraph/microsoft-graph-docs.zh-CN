---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1890ca9fb4777340ef69da815ae23e112472de2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016608"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCloudPcOnPremisesConnection()
displayName := "Display Name value"
requestBody.SetDisplayName(&displayName)
subscriptionId := "0ac520ee-14c0-480f-b6c9-0a90c585ffff"
requestBody.SetSubscriptionId(&subscriptionId)
subscriptionName := "Subscription Name value"
requestBody.SetSubscriptionName(&subscriptionName)
adDomainName := "Active Directory Domain Name value"
requestBody.SetAdDomainName(&adDomainName)
adDomainUsername := "Active Directory Domain User Name value"
requestBody.SetAdDomainUsername(&adDomainUsername)
organizationalUnit := "Organization Unit value"
requestBody.SetOrganizationalUnit(&organizationalUnit)
resourceGroupId := "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG"
requestBody.SetResourceGroupId(&resourceGroupId)
virtualNetworkId := "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet"
requestBody.SetVirtualNetworkId(&virtualNetworkId)
subnetId := "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default"
requestBody.SetSubnetId(&subnetId)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
}
options := &msgraphsdk.OnPremisesConnectionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnections().Post(options)


```