---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25db3463cf71ddabc43675fe78fd79bfbce66fa1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960078"
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