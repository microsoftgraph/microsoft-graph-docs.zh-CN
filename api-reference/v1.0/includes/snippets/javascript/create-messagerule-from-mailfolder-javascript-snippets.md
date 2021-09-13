---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46b6fd5ac223ca721ff2763b71b94514c6e8cc3ffb7e9890b1680cba7a8217f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220986"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: 'From partner',      
    sequence: 2,      
    isEnabled: true,          
    conditions: {
        senderContains: [
          'adele'       
        ]
     },
     actions: {
        forwardTo: [
          {
             emailAddress: {
                name: 'Alex Wilbur',
                address: 'AlexW@contoso.onmicrosoft.com'
              }
           }
        ],
        stopProcessingRules: true
     }    
};

await client.api('/me/mailFolders/inbox/messageRules')
    .post(messageRule);

```