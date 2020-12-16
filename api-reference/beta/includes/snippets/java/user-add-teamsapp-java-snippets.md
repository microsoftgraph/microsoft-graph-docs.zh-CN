---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0652ef7f181833f341549fb10a6c5f2fc7d68ccf
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692809"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallation userScopeTeamsAppInstallation = new UserScopeTeamsAppInstallation();
userScopeTeamsAppInstallation.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"));

graphClient.users("5b649834-7412-4cce-9e69-176e95a394f5").teamwork().installedApps()
    .buildRequest()
    .post(userScopeTeamsAppInstallation);

```