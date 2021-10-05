---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efeb509e5c3a703bc5a002880ff4885355d06bcfad08342357fbf74fb70feed7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161645"
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