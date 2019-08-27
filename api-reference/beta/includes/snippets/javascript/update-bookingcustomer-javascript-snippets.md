---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4e4cd2dd3c4d9ae035aa1c8643fca86c13f63844
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636577"
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
    .update(bookingCustomer);

```