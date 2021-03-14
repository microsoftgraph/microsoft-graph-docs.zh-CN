---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9573f11f1ce80cd282b2e14d5154bd0a43056e8d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785329"
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
         'user@odata.bind':'https://graph.microsoft.com/v1.0/users(\'0040b377-61d8-43db-94f5-81374122dc7e\')'
      }
   ]
};

await client.api('/teams')
    .post(team);

```