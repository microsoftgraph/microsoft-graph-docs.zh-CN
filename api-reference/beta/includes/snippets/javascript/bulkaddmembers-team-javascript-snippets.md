---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edd3b8153311a51ffa350fab5a9dfd4a0367a3496d6326bec177dc5495fb608a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101402"
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