---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24178e642aab3e4298ea679bbde15d4419cd2db7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938305"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKeySet = {
  id: "keyset1",
  keys: [
    {
      k: "k-value",
      x5c: [
        "x5c-value"
      ],
      x5t: "x5t-value",
      kty: "kty-value",
      use: "use-value",
      exp: 99,
      nbf: 99,
      kid: "kid-value",
      e: "e-value",
      n: "n-value",
      d: "d-value",
      p: "p-value",
      q: "q-value",
      dp: "dp-value",
      dq: "dq-value",
      qi: "qi-value"
    }
  ]
};

let res = await client.api('/trustFramework/keySets')
    .version('beta')
    .post(trustFrameworkKeySet);

```