---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f42aad42f2dfdc22b90e0750e4dbe41c639c6a95
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523398"
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

await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections
    .Request()
    .AddAsync(cloudPcOnPremisesConnection);

```