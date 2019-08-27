---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 53fb8df2381b2a3a618f55aadde25f07730c0ba9
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636732"
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
    .post(contact);

```