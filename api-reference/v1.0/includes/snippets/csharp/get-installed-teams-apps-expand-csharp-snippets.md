---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0793f317d18357f79d1865809085230e424811c
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = await graphClient.Teams["{id}"].InstalledApps["{id}"]
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```