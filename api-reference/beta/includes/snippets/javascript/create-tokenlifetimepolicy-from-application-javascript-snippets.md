---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2089d6ff5b52c77a9d1f691209156ac577426315
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782114"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  '@odata.id':'https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/applications/{id}/tokenLifetimePolicies')
    .version('beta')
    .post(tokenLifetimePolicy);

```