---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f18ed013b33fde79418997401c49a7f5a6bc1655
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467264"
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