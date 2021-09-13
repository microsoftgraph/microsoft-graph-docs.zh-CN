---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f1411fb33e4ec6c76e847d3ca25a3545c2f2cfd1546683e18ca5fe2845620bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903475"
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
    .post(message);

```