---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5beed4ff397d91f5e7d6fdce19a0044b561d518d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470458"
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