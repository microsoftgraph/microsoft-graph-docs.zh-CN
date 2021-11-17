---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c784739f118a35f0f5a663014663f8bd59cf71588d5c8d58b5ac2474496c292
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  use: 'sig',
  kty: 'RSA',
  nbf: 1508969811,
  exp: 1508969811
};

await client.api('/trustFramework/keySets/{id}/generateKey')
    .version('beta')
    .post(trustFrameworkKey);

```