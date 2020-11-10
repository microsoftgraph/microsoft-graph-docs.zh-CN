---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 531cbc12033fcef337031fb180ce33b8f83c7b51
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976632"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallation userScopeTeamsAppInstallation = new UserScopeTeamsAppInstallation();
userScopeTeamsAppInstallation.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"));

graphClient.users("{id}").teamwork().installedApps()
    .buildRequest()
    .post(userScopeTeamsAppInstallation);

```