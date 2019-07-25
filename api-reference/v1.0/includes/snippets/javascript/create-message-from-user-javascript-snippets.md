---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 77e9a3a47ea4ec5bc693726ebfa7c453688900a4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723206"
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
    .post({message : message});

```