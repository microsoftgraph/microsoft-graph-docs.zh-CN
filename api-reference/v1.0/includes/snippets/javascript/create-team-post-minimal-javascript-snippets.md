---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a503422525634b6c28a060ae2599383a217fc6a53b9846423ab57361614e4186
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903245"
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