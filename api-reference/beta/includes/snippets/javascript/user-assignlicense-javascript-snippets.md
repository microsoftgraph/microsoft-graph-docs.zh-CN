---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff2f279865ad01d9512618e710b61b83c794383b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  addLicenses: [
    {
      disabledPlans: [ '11b0131d-43c8-4bbb-b2c8-e80f9a50834a' ],
      skuId: 'skuId-value-1'
    },
    {
      disabledPlans: [ 'a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235' ],
      skuId: 'skuId-value-2'
    }
  ],
  removeLicenses: []
};

await client.api('/me/assignLicense')
    .version('beta')
    .post(user);

```