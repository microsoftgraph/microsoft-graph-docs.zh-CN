---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2eab839f5d10edd0da2fbde1b798b377e59304a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  '@odata.id':'https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/applications/{id}/tokenLifetimePolicies/$ref')
    .post(tokenLifetimePolicy);

```