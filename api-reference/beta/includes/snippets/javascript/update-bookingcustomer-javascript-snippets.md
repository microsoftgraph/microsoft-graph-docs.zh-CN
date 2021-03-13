---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59222b6eca6b8c7b5db113d6102b9bd8e482dbf3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794108"
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