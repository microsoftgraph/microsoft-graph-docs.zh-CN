---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0766c3b487fa4bbea3966468bafea3d08bc2d41
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2020
ms.locfileid: "48315281"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  group@odata.bind: "https://graph.microsoft.com/v1.0/groups('groupId')",
  channels: [
        {
            displayName: "Class Announcements 📢",
            isFavoriteByDefault: true
        },
        {
            displayName: "Homework 🏋️",
            isFavoriteByDefault: true,
        }
    ],
    memberSettings: {
        allowCreateUpdateChannels: false,
        allowDeleteChannels: false,
        allowAddRemoveApps: false,
        allowCreateUpdateRemoveTabs: false,
        allowCreateUpdateRemoveConnectors: false
    },
    installedApps: [
        {
            teamsApp@odata.bind: "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
        },
        {
            teamsApp@odata.bind: "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
        }
    ]
};

let res = await client.api('/teams')
    .version('beta')
    .post(team);

```