---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b359ee0df5d328796651e352f10b5b52bffb7450
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50474985"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserScopeTeamsAppInstallationCollectionPage installedApps = graphClient.users("{id}").teamwork().installedApps()
    .buildRequest()
    .expand("teamsAppDefinition($expand=bot)")
    .get();

```