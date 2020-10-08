---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7095ae8045fcb0142755fb4f30e02c7a4ab801c
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374051"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
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
    .post(team);

```