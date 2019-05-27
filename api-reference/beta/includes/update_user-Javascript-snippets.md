---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6fc26052e0b9848ceb750096bb949f343125d0e1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  assignedLicenses: [
    {
      disabledPlans: [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      skuId: "skuId-value"
    }
  ],
  assignedPlans: [
    {
      assignedDateTime: "2016-10-19T10:37:00Z",
      capabilityStatus: "capabilityStatus-value",
      service: "service-value",
      servicePlanId: "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  businessPhones: [
    "businessPhones-value"
  ],
  city: "city-value"
};

let res = await client.api('/me')
    .version('beta')
    .update({user : user});

```