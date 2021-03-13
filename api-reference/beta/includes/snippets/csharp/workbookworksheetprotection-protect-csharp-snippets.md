---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bee96e2f15ccc8b7bb8b4e5eaf2f2abab5025130
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var options = new WorkbookWorksheetProtectionOptions
{
    AllowFormatCells = true,
    AllowFormatColumns = true,
    AllowFormatRows = true,
    AllowInsertColumns = true,
    AllowInsertRows = true,
    AllowInsertHyperlinks = true,
    AllowDeleteColumns = true,
    AllowDeleteRows = true,
    AllowSort = true,
    AllowAutoFilter = true,
    AllowPivotTables = true
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Protection
    .Protect(options)
    .Request()
    .PostAsync();

```