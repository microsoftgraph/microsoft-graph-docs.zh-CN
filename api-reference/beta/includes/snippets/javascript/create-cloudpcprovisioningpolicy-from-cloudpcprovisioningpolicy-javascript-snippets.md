---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe36e06b13898a9a26d8390e6796149a7e0acc1b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcProvisioningPolicy = {
    '@odata.type': '#microsoft.graph.cloudPcProvisioningPolicy',
    description: 'Description value',
    displayName: 'Display Name value',
    domainJoinConfiguration: {
        domainJoinType: 'hybridAzureADJoin',
        onPremisesConnectionId: '16ee6c71-fc10-438b-88ac-daa1ccafffff'
    },
    id: '1d164206-bf41-4fd2-8424-a3192d39ffff',
    imageDisplayName: 'Windows-10 19h1-evd',
    imageId: 'MicrosoftWindowsDesktop_Windows-10_19h1-evd',
    imageType: 'gallery',
    onPremisesConnectionId: '4e47d0f6-6f77-44f0-8893-c0fe1701ffff'
};

await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies')
    .version('beta')
    .post(cloudPcProvisioningPolicy);

```