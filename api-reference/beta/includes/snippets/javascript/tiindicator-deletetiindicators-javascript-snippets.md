---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 204e8b0d78f979006d1887df8e027e5a52b3b8eb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798448"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const resultInfo = {
  value: [
    'id-value1',
    'id-value2'
  ]
};

await client.api('/security/tiIndicators/deleteTiIndicators')
    .version('beta')
    .post(resultInfo);

```