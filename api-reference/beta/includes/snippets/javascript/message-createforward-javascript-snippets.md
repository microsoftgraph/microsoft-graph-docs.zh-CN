---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f1bf7b1bb51672da8bd7194aac36c47e5c1cea6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607239"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  message:{  
    isDeliveryReceiptRequested: true,
    toRecipients:[
      {
        emailAddress: {
          address:"danas@contoso.onmicrosoft.com",
          name:"Dana Swope"
        }
      }
     ]
  },
  comment: "Dana, just want to make sure you get this; you'll need this if the project gets approved." 
};

let res = await client.api('/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward')
    .version('beta')
    .post(message);

```