---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df5fe86a585214b93ed9f57e020ee26de421ec3954c4420b62ef60920f8e69b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104017"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = new TeamsAppInstallation();
teamsAppInstallation.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"));

graphClient.chats("19:ea28e88c00e94c7786b065394a61f296@thread.v2").installedApps()
    .buildRequest()
    .post(teamsAppInstallation);

```