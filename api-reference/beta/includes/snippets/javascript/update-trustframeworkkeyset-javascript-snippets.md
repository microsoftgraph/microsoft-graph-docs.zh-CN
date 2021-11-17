---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98fc9fb2b4af5c403f81d9962246a9bc7e4cb5bb5fe1ab667d528be9b87d0c60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKeySet = {
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

await client.api('/trustFramework/keySets/{id}')
    .version('beta')
    .put(trustFrameworkKeySet);

```