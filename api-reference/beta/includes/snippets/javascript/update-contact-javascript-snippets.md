---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f559bfddc660daa271be42c0f325153382207249
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
    emailAddresses:[
        {
            type:"personal",
            name:"Pavel Bansky",
            address:"pavelb@adatum.onmicrosoft.com"
        },
        {
          address: "pavelb@fabrikam.onmicrosoft.com",
          name: "Pavel Bansky",
          type: "other",
          otherLabel: "Volunteer work"
        }
    ]
};

let res = await client.api('/me/contacts/AAMkADh6v5AAAvgTCEAAA=')
    .version('beta')
    .update({contact : contact});

```