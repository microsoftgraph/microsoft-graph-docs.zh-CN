---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c739d211da220396f4513376bcd6d325d84de53c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083910"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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