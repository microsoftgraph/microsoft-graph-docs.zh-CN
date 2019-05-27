---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1d1d3915f9dafb2fb78c7d46a8eb2bf7f892f4ce
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462374"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].PivotTables
    .RefreshAll()
    .Request()
    .PostAsync();

```