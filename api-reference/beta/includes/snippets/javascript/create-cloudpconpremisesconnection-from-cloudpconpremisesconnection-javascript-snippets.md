---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e01a86653889495e0dc3a5022d3334a97f955340
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcOnPremisesConnection = {
  '@odata.type': '#microsoft.graph.cloudPcOnPremisesConnection',
  displayName: 'test-canary-02',
  type: 'hybridAzureADJoin',
  subscriptionId: '0ac520ee-14c0-480f-b6c9-0a90c585ffff',
  subscriptionName: 'CPC customer 001 test subscription',
  adDomainName: 'contoso001.com',
  adDomainUsername: 'dcadmin',
  organizationalUnit: 'OU=Domain Controllers, DC=contoso001, DC=com',
  resourceGroupId: '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG',
  virtualNetworkId: '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET',
  subnetId: '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet'
};

await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections')
    .version('beta')
    .post(cloudPcOnPremisesConnection);

```