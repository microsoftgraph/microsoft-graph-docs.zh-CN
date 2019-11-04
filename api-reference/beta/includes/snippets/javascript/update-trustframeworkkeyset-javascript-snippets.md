---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7053f3a200278a073a43d81530b09fd7f790e4e6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKeySet = {
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

let res = await client.api('/trustFramework/keySets/{id}')
    .version('beta')
    .put(trustFrameworkKeySet);

```