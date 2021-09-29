---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5815f87d59a1bf3fb399495333996d2a73c6b46
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996726"
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
            'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'18a80140-b0fb-4489-b360-2f6efaf225a0\')'
        },
        {
            '@odata.type': 'microsoft.graph.aadUserConversationMember',
            roles: ['owner'],
            'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'86503198-b81b-43fe-81ee-ad45b8848ac9\')'
        }
    ]
};

await client.api('/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add')
    .post(actionResultPart);

```