---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35bd8c48b8d3ffece072d5b11e7afbcb21c561a1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351959"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOnPremisesConnection = new CloudPcOnPremisesConnection
{
    DisplayName = "test-canary-02",
    Type = CloudPcOnPremisesConnectionType.HybridAzureADJoin,
    SubscriptionId = "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
    SubscriptionName = "CPC customer 001 test subscription",
    AdDomainName = "contoso001.com",
    AdDomainUsername = "dcadmin",
    OrganizationalUnit = "OU=Domain Controllers, DC=contoso001, DC=com",
    ResourceGroupId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG",
    VirtualNetworkId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET",
    SubnetId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet"
};

await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections
    .Request()
    .AddAsync(cloudPcOnPremisesConnection);

```