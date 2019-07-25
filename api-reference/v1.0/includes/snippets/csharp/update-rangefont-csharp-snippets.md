---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b7f51419f9b4b7948f3ad2c3968f7881669ff24
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Bold = true,
    Color = "color-value",
    Italic = true,
    Name = "name-value",
    Size = 99,
    Underline = "underline-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```