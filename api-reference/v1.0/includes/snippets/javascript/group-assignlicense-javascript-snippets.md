---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d44ea0cf07d5e57cd51c3dc066cdb762d3648450
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
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

let res = await client.api('/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense')
    .post(group);

```