---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ccf44037e991ffb50930e6a37855e13bb83ed37
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690948"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserScopeTeamsAppInstallationCollectionPage installedApps = graphClient.users("5b649834-7412-4cce-9e69-176e95a394f5").teamwork().installedApps()
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```