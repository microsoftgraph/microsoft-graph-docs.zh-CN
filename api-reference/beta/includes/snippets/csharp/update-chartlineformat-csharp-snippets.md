---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23f28e3607a37e867ccf98150daaf6d3d2911bc3af45881d9dc5619d0b22d250
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartLineFormat = new WorkbookChartLineFormat
{
    Color = "color-value"
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.SeriesAxis.Format.Line
    .Request()
    .UpdateAsync(workbookChartLineFormat);

```