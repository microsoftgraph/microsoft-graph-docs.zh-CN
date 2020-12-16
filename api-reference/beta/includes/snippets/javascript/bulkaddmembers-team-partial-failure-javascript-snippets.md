---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b456baca6f3c9a9c9b3861b34886287a0b33c65
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689660"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const actionResultPart = {
    values: [
        {
            @odata.type: "microsoft.graph.aadUserConversationMember",
            roles:[],
            user@odata.bind: "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            @odata.type: "microsoft.graph.aadUserConversationMember",
            roles:["owner"],
            user@odata.bind: "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
};

let res = await client.api('/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add')
    .version('beta')
    .post(actionResultPart);

```