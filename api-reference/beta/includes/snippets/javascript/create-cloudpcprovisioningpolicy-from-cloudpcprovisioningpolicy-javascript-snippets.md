---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07b224a0dcf25f943399577d11c321db3919f093
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523171"
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
  onPremisesConnectionId: "6bf90392-5fea-459a-9e9d-a2484abbffff",
  imageId: "Image ID value",
  imageDisplayName: "Image Display Name value",
  imageType: "gallery"
};

let res = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies')
    .version('beta')
    .post(cloudPcProvisioningPolicy);

```