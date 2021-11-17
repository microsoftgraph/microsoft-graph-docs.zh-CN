---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5851c81d0d33b00520b22d1d8c3c183b454055d9fa625319e6dc9c8dedd00b0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329059"
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