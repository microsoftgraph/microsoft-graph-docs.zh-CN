---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5beed4ff397d91f5e7d6fdce19a0044b561d518d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversation = {
    topic:"New locations for this quarter",
    threads:[
        {
            posts:[
                {
                    body:{
                        contentType:"html",
                        content:"What do we know so far?"
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
    .post({conversation : conversation});

```