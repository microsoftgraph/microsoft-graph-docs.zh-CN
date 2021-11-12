---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5af15d8627cd1bdd0363e7d799ad9a9fe072a3742c5c1783c94e9539eb0cad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartGridlines = new WorkbookChartGridlines
{
    Visible = true
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Axes.ValueAxis.MinorGridlines
    .Request()
    .UpdateAsync(workbookChartGridlines);

```