---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48a74f4c8d186dff537c1640f501b85cdab672a9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799343"
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
  onPremisesConnectionId: '6bf90392-5fea-459a-9e9d-a2484abbffff',
  imageId: 'Image ID value',
  imageDisplayName: 'Image Display Name value',
  imageType: 'gallery'
};

await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies')
    .version('beta')
    .post(cloudPcProvisioningPolicy);

```