---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d72c3861909edae72fba3d92d7880bc230a3f88
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "ColumnStacked";

var sourceData = JsonDocument.Parse(@"""A1:B1""");

var seriesBy = "Auto";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts
    .Add(type,seriesBy,sourceData)
    .Request()
    .PostAsync();

```