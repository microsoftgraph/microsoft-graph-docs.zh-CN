---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aecfddec9145cc0f41e5051783c5a750dbecba4
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("id eq '876df28f-2e78-423b-94a5-44181bd0e225',")
    .Expand("appDefinitions")
    .GetAsync();

```