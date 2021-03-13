---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1824bd8fddd4f79b189ae56e87c26c47a6501871
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779564"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingCustomer = {
    displayName: 'Joni Sherman',
    emailAddress: 'jonis@relecloud.com'
};

await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers')
    .version('beta')
    .post(bookingCustomer);

```