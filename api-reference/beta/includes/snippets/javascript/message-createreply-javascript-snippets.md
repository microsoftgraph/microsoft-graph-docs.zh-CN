---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8358e029e10ee2d33dd807d79dbd969376b58057
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  message:{  
    toRecipients:[
      {
        emailAddress: {
          address:"samanthab@contoso.onmicrosoft.com",
          name:"Samantha Booth"
        }
      },
      {
        emailAddress:{
          address:"randiw@contoso.onmicrosoft.com",
          name:"Randi Welch"
        }
      }
     ]
  },
  comment: "Samantha, Randi, would you name the group if the project is approved, please?" 
};

let res = await client.api('/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply')
    .version('beta')
    .post(message);

```