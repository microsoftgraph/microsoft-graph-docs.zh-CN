---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dc9e424811aea2781da520f0dc3fdee4697d6a4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328568"
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
result, err := graphClient.DeviceManagement().VirtualEndpoint().OnPremisesConnections().Post(requestBody)


```