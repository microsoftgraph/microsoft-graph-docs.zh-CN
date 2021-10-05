---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0818408f33cf46bd923a485d33177d89225b57ac036cb52fe73d91c9d8e3d077
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215764"
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