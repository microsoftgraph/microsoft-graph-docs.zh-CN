---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e510655794007163baf33c063f55b699017cca19f6bd5cfcb531d54f6c6ff42d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105038"
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