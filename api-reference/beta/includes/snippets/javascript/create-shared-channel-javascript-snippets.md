---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bd53349592dc96861067769fe10235cd453a1bf
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: 'My First Shared Channel',
  description: 'This is my first shared channel',
  membershipType: 'shared',
  members: [
    {
      '@odata.type': '#microsoft.graph.aadUserConversationMember',
      'user@odata.bind': 'https://graph.microsoft.com/beta/users(\'7640023f-fe43-gv3f-9gg4-84a9efe4acd6\')',
      roles: [
        'owner'
      ]
    }
  ]
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .version('beta')
    .post(channel);

```