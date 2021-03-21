---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e448f6ffee58076de0a5c9c1829e0e643b29b760
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chat = {
  chatType: 'group',
  topic: 'Group chat title',
  members: [
    {
      '@odata.type': '#microsoft.graph.aadUserConversationMember',
      roles: ['owner'],
      'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca\')'
    },
    {
      '@odata.type': '#microsoft.graph.aadUserConversationMember',
      roles: ['owner'],
      'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'82fe7758-5bb3-4f0d-a43f-e555fd399c6f\')'
    },
    {
      '@odata.type': '#microsoft.graph.aadUserConversationMember',
      roles: ['owner'],
      'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'3626a173-f2bc-4883-bcf7-01514c3bfb82\')'
    }
  ]
};

await client.api('/chats')
    .post(chat);

```