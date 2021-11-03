---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83515cf28c5664cdcba8440bf2a5cbe8bb173f02
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695732"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   'template@odata.bind':'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')',
   displayName: 'My Sample Team',
   description: 'My Sample Team’s Description',
   members: [
      {
         '@odata.type':'#microsoft.graph.aadUserConversationMember',
         roles: [
            'owner'
         ],
         'user@odata.bind':'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')'
      }
   ]
};

await client.api('/teams')
    .post(team);

```