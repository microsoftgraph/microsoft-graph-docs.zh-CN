---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 549375ceb1c1b46ba64a3494d6305167e30572d5b47b81964553ad0950a5ad18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxisTitle = new WorkbookChartAxisTitle
{
    Text = "text-value",
    Visible = true
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.ValueAxis.Title
    .Request()
    .UpdateAsync(workbookChartAxisTitle);

```