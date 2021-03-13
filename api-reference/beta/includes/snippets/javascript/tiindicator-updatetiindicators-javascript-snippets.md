---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a67f19889721770a31cf2c3b78999b9a8e1a9293
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796645"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  value: [
    {
      id: 'c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4',
      additionalInformation: 'mytest'
    },
    {
      id: 'e58c072b-c9bb-a5c4-34ce-eb69af44fb1e',
      additionalInformation: 'test again'
    }
  ]
};

await client.api('/security/tiIndicators/updateTiIndicators')
    .version('beta')
    .post(tiIndicator);

```