---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 503c14c6f5df385616e106bb44dbde30d6bfc75a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129992"
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

await client.api('/bookingBusinesses/fabrikam@contoso.onmicrosoft.com')
    .version('beta')
    .update(bookingBusiness);

```