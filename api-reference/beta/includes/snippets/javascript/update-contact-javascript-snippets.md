---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc29d6e366698e0e910c67d44021cdc9c3d513f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
    emailAddresses: [
        {
            type: 'personal',
            name: 'Pavel Bansky',
            address: 'pavelb@adatum.onmicrosoft.com'
        },
        {
          address: 'pavelb@fabrikam.onmicrosoft.com',
          name: 'Pavel Bansky',
          type: 'other',
          otherLabel: 'Volunteer work'
        }
    ]
};

await client.api('/me/contacts/AAMkADh6v5AAAvgTCEAAA=')
    .version('beta')
    .update(contact);

```