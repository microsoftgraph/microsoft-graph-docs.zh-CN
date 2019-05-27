---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 05cec4f7392df8912b24802bf553a4b31137bfbe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478466"
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