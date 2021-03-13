---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08be3aa2d18d5b8b08f45924881442723af16874
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783666"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartTitle = new WorkbookChartTitle
{
    Overlay = true,
    Text = "text-value",
    Visible = true
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Title
    .Request()
    .UpdateAsync(workbookChartTitle);

```