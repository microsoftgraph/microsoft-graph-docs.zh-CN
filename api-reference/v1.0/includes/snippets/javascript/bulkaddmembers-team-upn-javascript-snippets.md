---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c77c53a3e8bea1f0832da3f958a4fa87c60a776b
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688406"
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
            'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')'
        },
        {
            '@odata.type': 'microsoft.graph.aadUserConversationMember',
            roles: ['owner'],
            'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'alex@contoso.com\')'
        }
    ]
};

await client.api('/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add')
    .post(actionResultPart);

```