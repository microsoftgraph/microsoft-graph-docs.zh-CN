---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af9afe94afdb9e375e3a2ba34d403d1bda5f961a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955093"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallation userScopeTeamsAppInstallation = graphClient.users("5b649834-7412-4cce-9e69-176e95a394f5").teamwork().installedApps("NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=")
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```