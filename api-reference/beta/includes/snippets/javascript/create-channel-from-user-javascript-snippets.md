---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3e840279bbf4939c200114777a7aac1fc881d7b
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512255"
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
           user@odata.bind:"https://graph.microsoft.com/beta/users('{user_id}')",
           roles:["owner"]
        }
     ]
};

let res = await client.api('/teams/{group_id}/channels')
    .version('beta')
    .post(channel);

```