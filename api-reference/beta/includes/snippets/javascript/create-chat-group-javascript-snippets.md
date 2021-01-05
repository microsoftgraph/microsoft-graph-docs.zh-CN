---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4695accdf80f45ebdb415df483cf7ebcbe35a01a
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chat = {
  chatType: "group",
  topic: "Group chat title",
  members: [
    {
      @odata.type: "#microsoft.graph.aadUserConversationMember",
      roles: ["owner"],
      user@odata.bind: "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"
    },
    {
      @odata.type: "#microsoft.graph.aadUserConversationMember",
      roles: ["owner"],
      user@odata.bind: "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"
    },
    {
      @odata.type: "#microsoft.graph.aadUserConversationMember",
      roles: ["owner"],
      user@odata.bind: "https://graph.microsoft.com/beta/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')"
    }
  ]
};

let res = await client.api('/chats')
    .version('beta')
    .post(chat);

```