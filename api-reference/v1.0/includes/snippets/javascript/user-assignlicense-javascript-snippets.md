---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d4a7dd06921208c8ca060cc2d940a15d3d577617
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715195"
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
      skuId: "guid"
    }
  ],
  removeLicenses: [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
};

let res = await client.api('/me/assignLicense')
    .post(user);

```