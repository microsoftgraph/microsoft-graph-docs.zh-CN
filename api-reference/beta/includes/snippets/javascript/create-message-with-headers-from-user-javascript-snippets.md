---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13449fdd1245f1af4c44ba1288f335fca89a3e90
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    subject: '9/8/2018: concert',
    body: {
        contentType: 'HTML',
        content: 'The group represents Washington.'
    },
    toRecipients: [
        {
            emailAddress: {
                address: 'AlexW@contoso.OnMicrosoft.com'
            }
        }
    ],
    internetMessageHeaders: [
        {
            name: 'x-custom-header-group-name',
            value: 'Washington'
        },
        {
            name: 'x-custom-header-group-id',
            value: 'WA001'
        }
    ]
};

await client.api('/me/messages')
    .version('beta')
    .post(message);

```