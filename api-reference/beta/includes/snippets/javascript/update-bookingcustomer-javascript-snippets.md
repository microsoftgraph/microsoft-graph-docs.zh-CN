---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 240318e3d0a95e141fc178ce910dc51ef71457c1124f73eeca50fd550117f37d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903120"
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

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a')
    .version('beta')
    .update(bookingCustomer);

```