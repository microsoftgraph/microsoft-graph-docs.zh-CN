---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e59bd3bfaf079235608b5e7cafb60b32b98b3fc5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: 'busy'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject')
    .version('beta')
    .post(reject);

```