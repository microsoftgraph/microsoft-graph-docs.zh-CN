---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9f1bf7b1bb51672da8bd7194aac36c47e5c1cea6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478478"
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