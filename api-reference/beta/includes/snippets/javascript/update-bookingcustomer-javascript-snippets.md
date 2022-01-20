---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a04d10e19a4aff86213a36e0afa0443f4e3d797
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094580"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingCustomer = {
    displayName: 'Adele',
    emailAddress: 'adele@relecloud.com'
};

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a')
    .version('beta')
    .update(bookingCustomer);

```