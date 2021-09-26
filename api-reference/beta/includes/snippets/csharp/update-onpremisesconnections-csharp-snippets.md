---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62344f717937c8035f86ca81b1e268f2696d2db70fd6045f4dc67adbe55e4ed5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278420"
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