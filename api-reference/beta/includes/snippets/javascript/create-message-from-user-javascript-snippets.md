---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 16325749053d48b544e3e4ebdfbfd3627d332b89
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    subject:"Did you see last night's game?",
    importance:"Low",
    body:{
        contentType:"HTML",
        content:"They were <b>awesome</b>!"
    },
    toRecipients:[
        {
            emailAddress:{
                address:"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ]
};

let res = await client.api('/me/messages')
    .version('beta')
    .post({message : message});

```