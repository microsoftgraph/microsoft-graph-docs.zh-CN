---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 068e207d5ef335b5480a2f88e5b04fdf67c616e8
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   template@odata.bind:"https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
   group@odata.bind:"https://graph.microsoft.com/v1.0/groups('groupId')",
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
    .post(team);

```