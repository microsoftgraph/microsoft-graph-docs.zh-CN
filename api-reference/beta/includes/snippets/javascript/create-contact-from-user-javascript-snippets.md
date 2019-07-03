---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0e8fa04fa0375084b2dab3155e468b0bad7591e0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521289"
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
      address: "pavelb@contoso.onmicrosoft.com",
      name: "Pavel Bansky",
      type: "personal"
    },
    {
      address: "pavelb@fabrikam.onmicrosoft.com",
      name: "Pavel Bansky",
      type: "other",
      otherLabel: "Volunteer work"
    }
  ],
  "phones" : [
    {
      number: "+1 732 555 0102",
      type: "business"
    }
  ]
};

let res = await client.api('/me/contacts')
    .version('beta')
    .post({contact : contact});

```