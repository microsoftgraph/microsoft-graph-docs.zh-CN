---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 434a67c82405d35b36cdd5ad9285c2b2efda905d
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "36636675"
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
    .post(messageRule);

```