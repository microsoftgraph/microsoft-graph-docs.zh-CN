---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 791c77ba3afa4971cb654532220e3138f85d61b1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  value: [
    {
      id: "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      additionalInformation: "mytest"
    },
    {
      id: "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
      additionalInformation: "test again"
    }
  ]
};

let res = await client.api('/security/tiIndicators/updateTiIndicators')
    .version('beta')
    .post(tiIndicator);

```