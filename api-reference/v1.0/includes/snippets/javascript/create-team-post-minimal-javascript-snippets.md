---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 518648d60d2e21bb28f2cc421d3e2ef5c38cf5f3
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48907308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   template@odata.bind:"https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
   displayName:"My Sample Team",
   description:"My Sample Team’s Description",
   members:[
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
    .post(team);

```