---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d5127d3d57f7e9054f8978c32ca623176f27e63369edb48c4db6cde9d4bf859
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215942"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = new TeamsAppInstallation();
teamsAppInstallation.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"));

graphClient.teams("87654321-0abc-zqf0-321456789q").installedApps()
    .buildRequest()
    .post(teamsAppInstallation);

```