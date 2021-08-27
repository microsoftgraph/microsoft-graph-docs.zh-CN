---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43a3265fc09328979286e0631de35539d31efc9aa9557b0a94321d2dc2f3bd76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
    body: {
        contentType: 'html',
        content: '<div><div><at id=\"0\">TestTag</at>&nbsp;Testing Tags</div></div>'
    },
    mentions: [
        {
            id: 0,
            mentionText: 'TestTag',
            mentioned: {
                tag: {
                    id: 'MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM2OGEzZTM2NS1mN2Q5LTRhNTYtYjQ5OS0yNDMzMmE5Y2M1NzIjI3RTMERJZ1Z1ZQ==',
                    displayName: 'TestTag'
                }
            }
        }
    ]
};

await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages')
    .version('beta')
    .post(chatMessage);

```