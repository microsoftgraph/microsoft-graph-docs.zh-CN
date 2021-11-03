---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0149efb4ff95e13b9f5433e5538e7c83a9aafed6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696383"
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
      'user@odata.bind': 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')'
    },
    {
      '@odata.type': '#microsoft.graph.aadUserConversationMember',
      roles: ['owner'],
      'user@odata.bind': 'https://graph.microsoft.com/beta/users(\'alex@contoso.com\')'
    }
  ]
};

await client.api('/chats')
    .version('beta')
    .post(chat);

```