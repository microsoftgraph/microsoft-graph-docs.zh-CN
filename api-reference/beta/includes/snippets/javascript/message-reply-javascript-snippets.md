---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c3bde045b81c501b1649b0abec770a3586420ebe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
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
  comment: "Samantha, Randi, would you name the group please?" 
};

let res = await client.api('/me/messages/AAMkADA1MTAAAAqldOAAA=/reply')
    .version('beta')
    .post(reply);

```