---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d932516807eecd66f73a36b1ee94499ed304a1a
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const acquireAccessToken = {
  credentials: [
    {
      @odata.type: "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
};

let res = await client.api('/applications/{applicationsId}/synchronization/acquireAccessToken')
    .version('beta')
    .post(acquireAccessToken);

```