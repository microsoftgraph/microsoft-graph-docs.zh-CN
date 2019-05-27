---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fb4fd2977a1489975a053f29b201a26bc9a40525
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookPivotTable = await graphClient.Drive.Root.Workbook.Worksheets["{id}"].PivotTables["{id}"]
    .Request()
    .GetAsync();

```