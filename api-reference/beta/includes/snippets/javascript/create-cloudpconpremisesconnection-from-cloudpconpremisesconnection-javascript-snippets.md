---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f94e4f6854c25afe2dd3d385bcd9a7fbfd70399e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcOnPremisesConnection = {
  '@odata.type': '#microsoft.graph.cloudPcOnPremisesConnection',
  displayName: 'Display Name value',
  subscriptionId: '0ac520ee-14c0-480f-b6c9-0a90c585ffff',
  subscriptionName: 'Subscription Name value',
  adDomainName: 'Active Directory Domain Name value',
  adDomainUsername: 'Active Directory Domain User Name value',
  organizationalUnit: 'Organization Unit value',
  resourceGroupId: '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG',
  virtualNetworkId: '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet',
  subnetId: '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default'
};

await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections')
    .version('beta')
    .post(cloudPcOnPremisesConnection);

```