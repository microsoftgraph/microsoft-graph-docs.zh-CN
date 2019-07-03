---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ce52c1078ef5427805f51c80d14016c142440bfc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingCustomer = {
    displayName: "Adele",
    emailAddress: "adele@relecloud.com"
};

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a')
    .version('beta')
    .update({bookingCustomer : bookingCustomer});

```