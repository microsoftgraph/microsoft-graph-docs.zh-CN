---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a6e35255fa6e78c61b33124b218ffe7a0b39bab
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125101"
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

New-MgDeviceManagementVirtualEndpointOnPremisesConnection -BodyParameter $params

```