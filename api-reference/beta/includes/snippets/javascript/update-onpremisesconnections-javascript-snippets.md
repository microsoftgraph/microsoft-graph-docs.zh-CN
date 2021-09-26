---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d4d9ef39ae7264dea69cea334394ec59ac4632fb72c531fc57913262cc3d72b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278421"
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

await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{id}')
    .version('beta')
    .update(cloudPcOnPremisesConnection);

```