---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 742477d445dc5abdec57a9f913c960827298a5c3f200322ae0b6cd01c8e563fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279692"
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
           'user@odata.bind':'https://graph.microsoft.com/v1.0/users(\'62855810-484b-4823-9e01-60667f8b12ae\')',
           roles: ['owner']
        }
     ]
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .post(channel);

```