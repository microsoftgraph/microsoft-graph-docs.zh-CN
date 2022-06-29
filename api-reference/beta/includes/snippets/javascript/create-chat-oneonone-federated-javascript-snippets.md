---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7caf1d1b744faf9eb3b86dffc3835d66002d278c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436854"
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
      'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'82af01c5-f7cc-4a2e-a728-3a5df21afd9d\')',
      tenantId: '4dc1fe35-8ac6-4f0d-904a-7ebcd364bea1'
    }
  ]
};

await client.api('/chats')
    .post(chat);

```