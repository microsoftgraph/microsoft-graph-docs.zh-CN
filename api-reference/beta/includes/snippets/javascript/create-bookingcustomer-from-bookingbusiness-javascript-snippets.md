---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 531362d928f55c3a42ab587a0958deb3dc51679b806eeb31878b4ab7c388bfa8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903142"
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