---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 670d3ff0fac85d37581a60fc8b2a94efe4903893
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingBusiness = {
  email: "admin@fabrikam.com",
  schedulingPolicy: {
      timeSlotInterval: "PT60M",
      minimumLeadTime: "P1D",
      maximumAdvance: "P30D",
      sendConfirmationsToOwner: true,
      allowStaffSelection: true
  }
};

let res = await client.api('/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com')
    .version('beta')
    .update({bookingBusiness : bookingBusiness});

```