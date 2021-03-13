---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4253be3a1fa358e9865170c2428c48dcc3c1b82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799642"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  '@odata.id':'https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/applications/{id}/tokenIssuancePolicies/$ref')
    .version('beta')
    .post(tokenIssuancePolicy);

```