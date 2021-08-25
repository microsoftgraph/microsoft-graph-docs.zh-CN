---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a21292f029a8652b13fca1829d04613064cc02e
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513249"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  addLicenses: [
    {
      disabledPlans: [
        '113feb6c-3fe4-4440-bddc-54d774bf0318',
        '14ab5db5-e6c4-4b20-b4bc-13e36fd2227f'
      ],
      skuId: 'b05e124f-c7cc-45a0-a6aa-8cf78c946968'
    },
    {
      disabledPlans: [
        'a413a9ff-720c-4822-98ef-2f37c2a21f4c'
      ],
      skuId: 'c7df2760-2c81-4ef7-b578-5b5392b571df'
    }
  ],
  removeLicenses: []
};

await client.api('/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/assignLicense')
    .version('beta')
    .post(group);

```