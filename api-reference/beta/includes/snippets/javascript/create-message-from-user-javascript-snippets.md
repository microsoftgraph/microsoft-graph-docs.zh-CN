---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fa811474cc8588b5f29e2bdeea983fc064cbb2b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795638"
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
    .version('beta')
    .post(message);

```