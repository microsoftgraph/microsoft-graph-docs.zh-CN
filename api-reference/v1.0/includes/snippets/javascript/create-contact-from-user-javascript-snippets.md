---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 688d4380749507e2eb0183a8d045001da431f296
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  givenName: 'Pavel',
  surname: 'Bansky',
  emailAddresses: [
    {
      address: 'pavelb@fabrikam.onmicrosoft.com',
      name: 'Pavel Bansky'
    }
  ],
  businessPhones: [
    '+1 732 555 0102'
  ]
};

await client.api('/me/contacts')
    .post(contact);

```