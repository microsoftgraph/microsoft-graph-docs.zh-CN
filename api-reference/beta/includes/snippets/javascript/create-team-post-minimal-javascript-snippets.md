---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09e6ab572f1a03f091a3a6be715628480b9f4141
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462517"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   template@odata.bind:"https://graph.microsoft.com/beta/teamsTemplates('standard')",
   displayName:"My Sample Team",
   description:"My Sample Team’s Description",
   members@odata.bind:[
      {
         @odata.type:"#microsoft.graph.aadUserConversationMember",
         roles:[
            "owner"
         ],
         userId:"0040b377-61d8-43db-94f5-81374122dc7e"
      }
   ]
};

let res = await client.api('/teams')
    .version('beta')
    .post(team);

```