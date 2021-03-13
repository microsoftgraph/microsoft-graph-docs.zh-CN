---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc705f6fe158184cf872889fc4b26e2af84068fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   'template@odata.bind':'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')',
   displayName: 'My Sample Team',
   description: 'My Sample Team’s Description',
   members: [
      {
         '@odata.type':'#microsoft.graph.aadUserConversationMember',
         roles: [
            'owner'
         ],
         'user@odata.bind':'https://graph.microsoft.com/beta/users(\'0040b377-61d8-43db-94f5-81374122dc7e\')'
      }
   ]
};

await client.api('/teams')
    .version('beta')
    .post(team);

```