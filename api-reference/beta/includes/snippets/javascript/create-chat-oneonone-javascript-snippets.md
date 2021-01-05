---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a3124a7764411e6f550422579005f40b202e085
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chat = {
  chatType: "oneOnOne",
  members: [
    {
      @odata.type: "#microsoft.graph.aadUserConversationMember",
      roles: ["owner"],
      user@odata.bind: "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
    },
    {
      @odata.type: "#microsoft.graph.aadUserConversationMember",
      roles: ["owner"],
      user@odata.bind: "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
    }
  ]
};

let res = await client.api('/chats')
    .version('beta')
    .post(chat);

```