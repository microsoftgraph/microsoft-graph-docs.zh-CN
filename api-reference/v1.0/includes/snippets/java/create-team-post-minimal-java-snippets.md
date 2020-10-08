---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d34697b17b8059f5b224f7ac80fbca2573cd9977
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374042"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/teamsTemplates('standard')"));
team.displayName = "My Sample Team";
team.description = "My Sample Team’s Description";
team.additionalDataManager().put("members@odata.bind", new JsonPrimitive("[
  {
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": [
      "owner"
    ],
    "userId": "0040b377-61d8-43db-94f5-81374122dc7e"
  }
]"));

graphClient.teams()
    .buildRequest()
    .post(team);

```