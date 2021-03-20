---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b538e42ae8c4022aea56904911c744cbfccaf501
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942251"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/teamsTemplates('educationClass')"));
team.displayName = "My Class Team";
team.description = "My Class Team’s Description";

graphClient.teams()
    .buildRequest()
    .post(team);

```