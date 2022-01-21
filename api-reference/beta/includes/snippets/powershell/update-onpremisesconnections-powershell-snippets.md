---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67e2d86e55e2945d68ceca69a2ae8e8548bbd2ce
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106710"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcOnPremisesConnection"
    DisplayName = "Display Name value"
    SubscriptionId = "0ac520ee-14c0-480f-b6c9-0a90c585ffff"
    SubscriptionName = "Subscription Name value"
    AdDomainName = "Active Directory Domain Name value"
    AdDomainUsername = "Active Directory Domain User Name value"
    OrganizationalUnit = "Organization Unit value"
    ResourceGroupId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG"
    VirtualNetworkId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet"
    SubnetId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default"
}

Update-MgDeviceManagementVirtualEndpointOnPremisesConnection -CloudPcOnPremisesConnectionId $cloudPcOnPremisesConnectionId -BodyParameter $params

```