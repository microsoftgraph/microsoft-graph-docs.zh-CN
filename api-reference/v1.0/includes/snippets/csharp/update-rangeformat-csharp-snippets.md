---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa858a7f15dd8f81f3ee7c0b213d4d8b063a190e52a8c7940e121d09b4912c92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105328"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = new WorkbookRangeFormat
{
    ColumnWidth = 135,
    VerticalAlignment = "Top",
    RowHeight = 49,
    WrapText = false
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("$A$1").Format
    .Request()
    .UpdateAsync(workbookRangeFormat);

```