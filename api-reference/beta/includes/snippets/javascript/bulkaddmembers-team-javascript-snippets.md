---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa0d79cf082cfe5d598bcf36ecb6caf5fe1205a6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803480"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const actionResultPart = {
    values: [
        {
            '@odata.type': 'microsoft.graph.aadUserConversationMember',
            roles: [],
            'user@odata.bind': 'https://graph.microsoft.com/beta/users(\'18a80140-b0fb-4489-b360-2f6efaf225a0\')'
        },
        {
            '@odata.type': 'microsoft.graph.aadUserConversationMember',
            roles: ['owner'],
            'user@odata.bind': 'https://graph.microsoft.com/beta/users(\'86503198-b81b-43fe-81ee-ad45b8848ac9\')'
        }
    ]
};

await client.api('/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add')
    .version('beta')
    .post(actionResultPart);

```