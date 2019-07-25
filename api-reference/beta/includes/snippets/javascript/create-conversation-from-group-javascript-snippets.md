---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dcf5fa000e0b85cc18a49b319af9f8f4c0a0b01a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711812"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversation = {
    topic:"New head count",
    threads:[
        {
            posts:[
                {
                    body:{
                        contentType:"html",
                        content:"The confirmation will come by the end of the week."
                    },
                    newParticipants:[
                        {
                            emailAddress:{
                                name:"Adele Vance",
                                address:"AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    ]
                }
            ]
        }
    ]
};

let res = await client.api('/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations')
    .version('beta')
    .post({conversation : conversation});

```