---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dab8551cc00d32af17edb451b84634eb234a8293
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    subject: 'Party planning',
    toRecipients: [
      {
          emailAddress: {
              name: 'Samantha Booth',
              address: 'samanthab@contoso.onmicrosoft.com'
          }
      }
    ],
    mentions: [
      {    
        mentioned: {
          name: 'Dana Swope',
          address: 'danas@contoso.onmicrosoft.com'
         }
      }
    ]
};

await client.api('/me/messages')
    .version('beta')
    .post(message);

```