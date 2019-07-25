---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 05cec4f7392df8912b24802bf553a4b31137bfbe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  givenName: "Pavel",
  surname: "Bansky",
  emailAddresses: [
    {
      address: "pavelb@fabrikam.onmicrosoft.com",
      name: "Pavel Bansky"
    }
  ],
  businessPhones: [
    "+1 732 555 0102"
  ]
};

let res = await client.api('/me/contacts')
    .post({contact : contact});

```