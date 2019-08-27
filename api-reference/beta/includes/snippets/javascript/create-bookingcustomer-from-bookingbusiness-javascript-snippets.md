---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d2c431d1c8fc9620ed9ad7edbde4d46c475035ff
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingCustomer = {
    displayName: "Joni Sherman",
    emailAddress: "jonis@relecloud.com"
};

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers')
    .version('beta')
    .post(bookingCustomer);

```