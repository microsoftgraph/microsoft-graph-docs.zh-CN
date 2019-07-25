---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b9a567112f98b0c265efd597e8d8976bf307c2b2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891991"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Italic = true,
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range('$B$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```