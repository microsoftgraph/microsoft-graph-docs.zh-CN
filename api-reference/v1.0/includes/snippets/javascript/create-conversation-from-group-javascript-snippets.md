---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9b186e551c1cef6365600f89ac085a9c89f5721
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversation = {
    topic: 'Take your wellness days and rest',
    threads: [
        {
            posts: [
                {
                    body: {
                        contentType: 'html',
                        content: 'Contoso cares about you: Rest and Recharge'
                    },
                    newParticipants: [
                        {
                            emailAddress: {
                                name: 'Adele Vance',
                                address: 'AdeleV@contoso.onmicrosoft.com'
                            }
                        }
                    ]
                }
            ]
        }
    ]
};

await client.api('/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations')
    .post(conversation);

```