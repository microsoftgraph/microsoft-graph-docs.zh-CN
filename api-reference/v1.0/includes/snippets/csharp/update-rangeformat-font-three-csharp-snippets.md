---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9eec6507ac82185a42d31ec1f3bb97be596633f1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737762"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Underline = "Single",
    Color = "#FFFFFF",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"].Range('$C$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```