---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d30f4755a136c2f85971fdf6074f6a22a0880692
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60684131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    roles: ['owner'],
    'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')'
};

await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .version('beta')
    .post(conversationMember);

```