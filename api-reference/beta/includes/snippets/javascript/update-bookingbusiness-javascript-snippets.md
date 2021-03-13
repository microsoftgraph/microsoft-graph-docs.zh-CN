---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f75c957019ad8248fefde99cb5df6b04e41eaf2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingBusiness = {
  email: 'admin@fabrikam.com',
  schedulingPolicy: {
      timeSlotInterval: 'PT60M',
      minimumLeadTime: 'P1D',
      maximumAdvance: 'P30D',
      sendConfirmationsToOwner: true,
      allowStaffSelection: true
  }
};

await client.api('/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com')
    .version('beta')
    .update(bookingBusiness);

```