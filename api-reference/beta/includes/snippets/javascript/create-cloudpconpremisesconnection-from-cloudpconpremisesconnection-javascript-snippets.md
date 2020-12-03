---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fde34bce11ae79c38e5c9d4fabae81cdedd2a386
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcOnPremisesConnection = {
  @odata.type: "#microsoft.graph.cloudPcOnPremisesConnection",
  displayName: "Display Name value",
  subscriptionId: "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  subscriptionName: "Subscription Name value",
  adDomainName: "Active Directory Domain Name value",
  adDomainUsername: "Active Directory Domain User Name value",
  organizationalUnit: "Organization Unit value",
  resourceGroupId: "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  virtualNetworkId: "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  subnetId: "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default"
};

let res = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections')
    .version('beta')
    .post(cloudPcOnPremisesConnection);

```