---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 931a403c6a68ba90fe82d859b79764118297771e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621365"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendMail = {
  Message: {
    subject: "Project kickoff",
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
  }
};

let res = await client.api('/me/sendMail')
    .version('beta')
    .post(sendMail);

```