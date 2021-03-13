---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a017ea179aa4a2192fe5ea23feff2fc54f67d0ce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const acquireAccessToken = {
  credentials: [
    {
      '@odata.type': 'microsoft.graph.synchronizationSecretKeyStringValuePair'
    }
  ]
};

await client.api('/applications/{applicationsId}/synchronization/acquireAccessToken')
    .version('beta')
    .post(acquireAccessToken);

```