---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b725784c3ea958308ff6b14f7a58579472095b53
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753827"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  @odata.type: "#Microsoft.Graph.channel",
  membershipType: "private",
  displayName: "My First Private Channel",
  description: "This is my first private channels",
  members:
     [
        {
           @odata.type:"#microsoft.graph.aadUserConversationMember",
           user@odata.bind:"https://graph.microsoft.com/beta/users('62855810-484b-4823-9e01-60667f8b12ae')",
           roles:["owner"]
        }
     ]
};

let res = await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .version('beta')
    .post(channel);

```