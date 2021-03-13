---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33164e8d70beb800d71b6c28f0d1967df91ee21e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKeySet = {
  id: 'keyset1',
  keys: [
    {
      k: 'k-value',
      x5c: [
        'x5c-value'
      ],
      x5t: 'x5t-value',
      kty: 'kty-value',
      use: 'use-value',
      exp: 99,
      nbf: 99,
      kid: 'kid-value',
      e: 'e-value',
      n: 'n-value',
      d: 'd-value',
      p: 'p-value',
      q: 'q-value',
      dp: 'dp-value',
      dq: 'dq-value',
      qi: 'qi-value'
    }
  ]
};

await client.api('/trustFramework/keySets')
    .version('beta')
    .post(trustFrameworkKeySet);

```