---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 181b976fef4e3abe3abd69b57ef8c6bb7d4ec758
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOnPremisesConnection = new CloudPcOnPremisesConnection
{
    DisplayName = "Display Name value",
    SubscriptionId = "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
    SubscriptionName = "Subscription Name value",
    AdDomainName = "Active Directory Domain Name value",
    AdDomainUsername = "Active Directory Domain User Name value",
    OrganizationalUnit = "Organization Unit value",
    ResourceGroupId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
    VirtualNetworkId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
    SubnetId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default"
};

await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["{cloudPcOnPremisesConnection-id}"]
    .Request()
    .UpdateAsync(cloudPcOnPremisesConnection);

```