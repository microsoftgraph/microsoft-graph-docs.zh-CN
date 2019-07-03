---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bb0487d0d129ac4a0a378eb7d198b94a6fdea8f6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479400"
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

let res = await client.api('/me/mailFolders/inbox/messagerules')
    .version('beta')
    .post({messageRule : messageRule});

```