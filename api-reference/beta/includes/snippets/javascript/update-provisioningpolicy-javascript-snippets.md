---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d9e1dc4e66478039e37f65a78d91733c5ed9768
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcProvisioningPolicy = {
  '@odata.type': '#microsoft.graph.cloudPcProvisioningPolicy',
  displayName: 'Display Name value',
  description: 'Description value',
  onPremisesConnectionId: '4e47d0f6-6f77-44f0-8893-c0fe1701ffff',
  imageId: 'Image ID value',
  imageDisplayName: 'Image Display Name value',
  imageType: 'custom'
};

await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}')
    .version('beta')
    .update(cloudPcProvisioningPolicy);

```