---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db53b0547b62577c1fe68d7d66205750175cd8d2
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')",
  displayName: "My Class Team",
  description: "My Class Team’s Description",
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