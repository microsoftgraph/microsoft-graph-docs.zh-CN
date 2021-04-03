---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60c7190fd65beb11d0faf37dfffd510ca36205ad
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508450"
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