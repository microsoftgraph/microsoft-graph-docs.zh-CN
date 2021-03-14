---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56c6ce8dbeb0d1a9dd337097515495f4a2155b6a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  '@odata.type': '#Microsoft.Graph.channel',
  membershipType: 'private',
  displayName: 'My First Private Channel',
  description: 'This is my first private channels',
  members: 
     [
        {
           '@odata.type':'#microsoft.graph.aadUserConversationMember',
           'user@odata.bind':'https://graph.microsoft.com/v1.0/users(\'{user_id}\')',
           roles: ['owner']
        }
     ]
};

await client.api('/teams/{group_id}/channels')
    .post(channel);

```