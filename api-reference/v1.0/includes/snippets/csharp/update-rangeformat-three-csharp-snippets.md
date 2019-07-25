---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b19d00890576f7f8ebaf591be63b17e19d1693c6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = new WorkbookRangeFormat
{
    ColumnWidth = 135,
    HorizontalAlignment = "Right",
    VerticalAlignment = "Top",
    RowHeight = 49,
    WrapText = false
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range('$C$1').Format
    .Request()
    .UpdateAsync(workbookRangeFormat);

```