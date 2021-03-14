---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fae806ba0792cba260c657a5873d22f34a24f4ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777905"
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