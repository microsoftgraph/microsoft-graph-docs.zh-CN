---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1883960370a2f87a53a4c6dfa590580789fcbc61
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694101"
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
    .post(conversationMember);

```