---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f18ed013b33fde79418997401c49a7f5a6bc1655
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeBorder = new WorkbookRangeBorder
{
    Color = "color-value",
    Style = "style-value",
    SideIndex = "sideIndex-value",
    Weight = "weight-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Borders["{sideIndex}"]
    .Request()
    .UpdateAsync(workbookRangeBorder);

```