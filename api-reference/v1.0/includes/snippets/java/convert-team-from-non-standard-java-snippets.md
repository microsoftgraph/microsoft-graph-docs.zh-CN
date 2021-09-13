---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ccfa153f3f91594b68d551f7f8bfaa75e92c31a56dbbcf3bc1d9ee58b3ea2ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903234"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')"));
team.displayName = "My Class Team";
team.description = "My Class Team’s Description";

graphClient.teams()
    .buildRequest()
    .post(team);

```