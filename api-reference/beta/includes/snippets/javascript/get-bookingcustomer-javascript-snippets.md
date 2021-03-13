---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54208b807ba1c506c083e81334ab5b4b1f46d139
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793438"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingCustomer = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a')
    .version('beta')
    .get();

```