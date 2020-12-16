---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfc8e8206b60e38e409cae7271efb66c87408903
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691196"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsAppInstallationCollectionPage installedApps = graphClient.teams("6903fa93-605b-43ef-920e-77c4729f8258").installedApps()
    .buildRequest()
    .get();

```