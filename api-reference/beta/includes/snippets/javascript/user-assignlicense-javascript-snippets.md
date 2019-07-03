---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6aa944b7b598c272020d6e26bb1d6f0ab452eb3d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478624"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  addLicenses: [
    {
      disabledPlans: [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      skuId: "skuId-value-1"
    },
    {
      disabledPlans: [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      skuId: "skuId-value-2"
    }
  ],
  removeLicenses: []
};

let res = await client.api('/me/assignLicense')
    .version('beta')
    .post(user);

```