---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0b893fe4f9e3bbbf2bf158f243b7a74518d48319
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: "From partner",      
    sequence: 2,      
    isEnabled: true,          
    conditions: {
        senderContains: [
          "adele"       
        ]
     },
     actions: {
        forwardTo: [
          {
             emailAddress: {
                name: "Alex Wilbur",
                address: "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        stopProcessingRules: true
     }    
};

let res = await client.api('/me/mailFolders/inbox/messageRules')
    .post({messageRule : messageRule});

```