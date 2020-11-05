---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e14d5a30ceb499278bb1bd00a657fb21836ca052
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48907256"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/teamsTemplates('standard')"));
team.displayName = "My Sample Team";
team.description = "My Sample Team’s Description";
LinkedList<ConversationMember> membersList = new LinkedList<ConversationMember>();
AadUserConversationMember members = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
members.roles = rolesList;
members.userId = "0040b377-61d8-43db-94f5-81374122dc7e";
membersList.add(members);
team.members = membersList;

graphClient.teams()
    .buildRequest()
    .post(team);

```