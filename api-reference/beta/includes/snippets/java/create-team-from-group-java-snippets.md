---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62409f03d58b7cfff7332ac1239e5df5d51b6b4a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942249"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/teamsTemplates('standard')"));
team.additionalDataManager().put("group@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/groups('groupId')"));

graphClient.teams()
    .buildRequest()
    .post(team);

```