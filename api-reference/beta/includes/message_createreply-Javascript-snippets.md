---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8358e029e10ee2d33dd807d79dbd969376b58057
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444060"
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