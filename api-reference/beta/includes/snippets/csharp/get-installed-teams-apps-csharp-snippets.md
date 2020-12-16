---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b2b066aa9d3a775be0217c21746954660be25ef
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692892"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = await graphClient.Teams["{id}"].InstalledApps["{id}"]
    .Request()
    .GetAsync();

```