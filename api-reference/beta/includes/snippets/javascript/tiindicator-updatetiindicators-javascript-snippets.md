---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 394be9542ab4cbb32963cf3148b2c8f676a1905324656d527f4769c51ffd5894
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220184"
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