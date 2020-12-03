---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fcc69d5c339465f0cde6a21d9e8521241a49bb5
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcProvisioningPolicy = {
  @odata.type: "#microsoft.graph.cloudPcProvisioningPolicy",
  displayName: "Display Name value",
  description: "Description value",
  onPremisesConnectionId: "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  imageId: "Image ID value",
  imageDisplayName: "Image Display Name value",
  imageType: "custom"
};

let res = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}')
    .version('beta')
    .update(cloudPcProvisioningPolicy);

```