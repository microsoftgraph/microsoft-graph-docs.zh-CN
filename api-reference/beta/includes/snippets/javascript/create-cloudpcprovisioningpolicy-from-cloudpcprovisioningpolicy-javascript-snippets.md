---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf27d30d17e591be99daa75669d1571bee170cf4
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759210"
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
    onPremisesConnectionId: '4e47d0f6-6f77-44f0-8893-c0fe1701ffff',
    windowsSettings: {
        language: 'en-US'
    }
};

await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies')
    .version('beta')
    .post(cloudPcProvisioningPolicy);

```