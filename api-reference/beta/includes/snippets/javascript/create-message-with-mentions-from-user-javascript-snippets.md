---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cd31bd4cd3f3d50d704224c1d1a3b6bb7a9f907e
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    subject: "Party planning",
    toRecipients:[
      {
          emailAddress:{
              name:"Samantha Booth",
              address:"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    mentions:[
      {    
        mentioned:{
          name:"Dana Swope",
          address:"danas@contoso.onmicrosoft.com"
         }
      }
    ]
};

let res = await client.api('/me/messages')
    .version('beta')
    .post(message);

```