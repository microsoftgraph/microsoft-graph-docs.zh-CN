---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 59c1e517b4fa3a55aa19392b193d6d9640311976
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466758"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{id}"].InstalledApps
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```