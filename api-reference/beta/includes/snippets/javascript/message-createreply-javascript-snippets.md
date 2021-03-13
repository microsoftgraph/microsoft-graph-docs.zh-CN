---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10fd5c85310f1d87853ecc3b85b10f5cff692243
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796199"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  message: {  
    toRecipients: [
      {
        emailAddress: {
          address: 'samanthab@contoso.onmicrosoft.com',
          name: 'Samantha Booth'
        }
      },
      {
        emailAddress: {
          address: 'randiw@contoso.onmicrosoft.com',
          name: 'Randi Welch'
        }
      }
     ]
  },
  comment: 'Samantha, Randi, would you name the group if the project is approved, please?' 
};

await client.api('/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply')
    .version('beta')
    .post(message);

```