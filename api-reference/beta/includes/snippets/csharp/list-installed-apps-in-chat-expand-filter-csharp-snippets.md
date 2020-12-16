---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eb858995342d48a63df65426590a189857481e7
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Chats["19:d65713bc498c4a428c71ef9353e6ce20@thread.v2"].InstalledApps
    .Request()
    .Filter("teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .Expand("teamsAppDefinition")
    .GetAsync();

```