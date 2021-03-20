---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee95cad7999e2e8934a07d801a1c55f272276a83
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969000"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = new TeamsAppInstallation();
teamsAppInstallation.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"));

graphClient.chats("19:ea28e88c00e94c7786b065394a61f296@thread.v2").installedApps()
    .buildRequest()
    .post(teamsAppInstallation);

```