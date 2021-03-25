---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d982e5453ac57846070adddd969d60911510e1e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209789"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallation userScopeTeamsAppInstallation = graphClient.users("5b649834-7412-4cce-9e69-176e95a394f5").teamwork().installedApps("NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=")
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```