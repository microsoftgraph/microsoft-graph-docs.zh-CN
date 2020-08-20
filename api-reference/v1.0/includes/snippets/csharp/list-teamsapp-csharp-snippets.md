---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aecfddec9145cc0f41e5051783c5a750dbecba4
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("id eq '876df28f-2e78-423b-94a5-44181bd0e225',")
    .Expand("appDefinitions")
    .GetAsync();

```