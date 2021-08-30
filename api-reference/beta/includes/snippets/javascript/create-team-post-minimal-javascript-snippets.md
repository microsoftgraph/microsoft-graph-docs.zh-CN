---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c593810aa3ff19d83dce54b360246322a250bbba37655bcb80fd93c717b97e09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378654"
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