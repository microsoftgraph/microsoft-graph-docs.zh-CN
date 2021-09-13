---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f140dc5a4d77d4a64f972795326ee1014d2f719e27ecc37a7ef217a7a5e0f271
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903472"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    subject: 'Did you see last night\'s game?',
    importance: 'Low',
    body: {
        contentType: 'HTML',
        content: 'They were <b>awesome</b>!'
    },
    toRecipients: [
        {
            emailAddress: {
                address: 'AdeleV@contoso.onmicrosoft.com'
            }
        }
    ]
};

await client.api('/me/messages')
    .post(message);

```