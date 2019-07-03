---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6167cbeca3eb19413553dbe34fa27c152ee85c26
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    subject:"9/8/2018: concert",
    body:{
        contentType:"HTML",
        content:"The group represents Washington."
    },
    toRecipients:[
        {
            emailAddress:{
                address:"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    internetMessageHeaders:[
        {
            name:"x-custom-header-group-name",
            value:"Washington"
        },
        {
            name:"x-custom-header-group-id",
            value:"WA001"
        }
    ]
};

let res = await client.api('/me/messages')
    .version('beta')
    .post({message : message});

```