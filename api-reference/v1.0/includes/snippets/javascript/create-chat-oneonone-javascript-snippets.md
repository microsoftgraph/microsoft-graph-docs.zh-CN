---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3722242b1537f1a2c9070d541b822a17a07229ed26908cb4319035497c85d768
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chat = {
  chatType: 'oneOnOne',
  members: [
    {
      '@odata.type': '#microsoft.graph.aadUserConversationMember',
      roles: ['owner'],
      'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'8b081ef6-4792-4def-b2c9-c363a1bf41d5\')'
    },
    {
      '@odata.type': '#microsoft.graph.aadUserConversationMember',
      roles: ['owner'],
      'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'82af01c5-f7cc-4a2e-a728-3a5df21afd9d\')'
    }
  ]
};

await client.api('/chats')
    .post(chat);

```