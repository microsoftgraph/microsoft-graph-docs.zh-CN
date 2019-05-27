---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 00f958fa57b6026ab08673861671ea2899cdde13
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440203"
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
    .post({message : message});

```