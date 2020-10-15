---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84f5de5ee7dac0978d1a8f22ca26e565f6c74624
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   template@odata.bind:"https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
   displayName:"My Class Team",
   description:"My Class Team’s Description",
   channels:[
      {
         displayName:"Class Announcements 📢",
         isFavoriteByDefault:true
      },
      {
         displayName:"Homework 🏋️",
         isFavoriteByDefault:true
      }
   ],
   memberSettings:{
      allowCreateUpdateChannels:false,
      allowDeleteChannels:false,
      allowAddRemoveApps:false,
      allowCreateUpdateRemoveTabs:false,
      allowCreateUpdateRemoveConnectors:false
   },
   installedApps:[
      {
         teamsApp@odata.bind:"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
      },
      {
         teamsApp@odata.bind:"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
      }
   ]
};

let res = await client.api('/teams')
    .version('beta')
    .post(team);

```