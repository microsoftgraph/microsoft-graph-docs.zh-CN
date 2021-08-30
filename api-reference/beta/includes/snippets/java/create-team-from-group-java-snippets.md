---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daa514c2af212efe27bdc49d935a85a503aada172835c86b93c6f6cb7d6cab21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378632"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/teamsTemplates('standard')"));
team.additionalDataManager().put("group@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"));

graphClient.teams()
    .buildRequest()
    .post(team);

```