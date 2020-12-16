---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 470ed9b1bf4bd817dcf43daa1a9a9cb84cc063fb
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692740"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = graphClient.teams("{id}").installedApps("{id}")
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```